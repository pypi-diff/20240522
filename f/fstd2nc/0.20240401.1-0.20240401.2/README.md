# Comparing `tmp/fstd2nc-0.20240401.1.tar.gz` & `tmp/fstd2nc-0.20240401.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fstd2nc-0.20240401.1.tar", last modified: Fri May  3 19:28:39 2024, max compression
+gzip compressed data, was "dist/fstd2nc-0.20240401.2.tar", last modified: Wed May 22 19:39:07 2024, max compression
```

## Comparing `fstd2nc-0.20240401.1.tar` & `fstd2nc-0.20240401.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.373991 fstd2nc-0.20240401.1/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1809 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/.gitignore
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.1/COPYING
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.1/COPYING.LESSER
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    30270 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/Changelog
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      114 2024-03-25 14:07:01.000000 fstd2nc-0.20240401.1/Makefile
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-05-03 19:28:39.373629 fstd2nc-0.20240401.1/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13489 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/README.md
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14775 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/README_fr.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.092862 fstd2nc-0.20240401.1/cccbuffer/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1022 2024-03-27 16:22:27.000000 fstd2nc-0.20240401.1/cccbuffer/_xarray_hook.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/cccdump.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.095437 fstd2nc-0.20240401.1/cccbuffer/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4101 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/ccc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/char.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/grid.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/levels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/superlabels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2024-04-23 18:55:54.000000 fstd2nc-0.20240401.1/cccbuffer/mixins/times.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.096648 fstd2nc-0.20240401.1/conda.recipe/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      658 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/conda.recipe/README.md
--rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)       67 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/conda.recipe/build.sh
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      512 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/conda.recipe/meta.yaml
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.185379 fstd2nc-0.20240401.1/debian/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      143 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/changelog
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        2 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/compat
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      624 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/control
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1103 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/copyright
--rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)      607 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/rules
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.185905 fstd2nc-0.20240401.1/debian/source/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       12 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/debian/source/format
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.187446 fstd2nc-0.20240401.1/fstd2nc/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3833 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9889 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7537 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/_xarray_hook.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    21835 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/extra.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.189999 fstd2nc-0.20240401.1/fstd2nc/locale/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1526 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/fstd2nc/locale/Makefile
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      974 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/fstd2nc/locale/README.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.043405 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.190428 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    25609 2024-05-03 19:26:40.000000 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    27563 2024-05-03 19:27:20.000000 fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA.po
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.373067 fstd2nc-0.20240401.1/fstd2nc/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    42803 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6457 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/accum.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/ascii.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20498 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/compat.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    11830 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/dates.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/diaghacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3220 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/ensembles.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    34534 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/extern.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3581 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/filter.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    12004 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/fstd.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23129 2024-05-03 18:43:18.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/gridhacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8248 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/masks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4249 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/mesh.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1786 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/misc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20973 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/netcdf.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/pruneaxes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/removestuff.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/select.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23171 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/series.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8075 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/sfc_codes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8783 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/vardict.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    41836 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/vcoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3499 2024-05-03 18:40:05.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/xmeta.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    61231 2024-04-19 14:45:18.000000 fstd2nc-0.20240401.1/fstd2nc/mixins/xycoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/fstd2nc/stdout.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-03 19:28:39.189068 fstd2nc-0.20240401.1/fstd2nc.egg-info/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1578 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/SOURCES.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/dependency_links.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      289 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/entry_points.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/requires.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2024-05-03 19:28:38.000000 fstd2nc-0.20240401.1/fstd2nc.egg-info/top_level.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.1/pyproject.toml
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1370 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.1/sample_meta.ini
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2024-05-03 19:28:39.374068 fstd2nc-0.20240401.1/setup.cfg
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2664 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.1/setup.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.440470 fstd2nc-0.20240401.2/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1809 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/.gitignore
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.2/COPYING
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.2/COPYING.LESSER
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    30715 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/Changelog
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      114 2024-03-25 14:07:01.000000 fstd2nc-0.20240401.2/Makefile
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-05-22 19:39:07.440209 fstd2nc-0.20240401.2/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13489 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/README.md
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14775 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/README_fr.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.424873 fstd2nc-0.20240401.2/cccbuffer/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1022 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/cccbuffer/_xarray_hook.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/cccdump.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.427416 fstd2nc-0.20240401.2/cccbuffer/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4101 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/cccbuffer/mixins/ccc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/mixins/char.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/mixins/grid.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/mixins/levels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.2/cccbuffer/mixins/superlabels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2024-04-23 18:55:54.000000 fstd2nc-0.20240401.2/cccbuffer/mixins/times.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.428508 fstd2nc-0.20240401.2/conda.recipe/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      658 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/conda.recipe/README.md
+-rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)       67 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/conda.recipe/build.sh
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      512 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/conda.recipe/meta.yaml
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.429863 fstd2nc-0.20240401.2/debian/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      143 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/debian/changelog
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        2 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/debian/compat
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      624 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/debian/control
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1103 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/debian/copyright
+-rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)      607 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/debian/rules
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.430247 fstd2nc-0.20240401.2/debian/source/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       12 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/debian/source/format
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.431454 fstd2nc-0.20240401.2/fstd2nc/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3833 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/fstd2nc/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9889 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7539 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/fstd2nc/_xarray_hook.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    21880 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/fstd2nc/extra.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.433660 fstd2nc-0.20240401.2/fstd2nc/locale/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1526 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.2/fstd2nc/locale/Makefile
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      974 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.2/fstd2nc/locale/README.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.378315 fstd2nc-0.20240401.2/fstd2nc/locale/fr_CA/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.433991 fstd2nc-0.20240401.2/fstd2nc/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    25691 2024-05-22 19:38:45.000000 fstd2nc-0.20240401.2/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    27563 2024-05-22 19:38:45.000000 fstd2nc-0.20240401.2/fstd2nc/locale/fr_CA.po
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.439797 fstd2nc-0.20240401.2/fstd2nc/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    42803 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6457 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/accum.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/ascii.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20498 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/compat.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    11830 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/dates.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/diaghacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3220 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/ensembles.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    34534 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/extern.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3581 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/filter.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    12202 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/fstd.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23688 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/gridhacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8248 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/masks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4249 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/mesh.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1786 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/misc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20990 2024-05-22 19:36:48.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/netcdf.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/pruneaxes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/removestuff.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/select.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23171 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/series.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8075 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/sfc_codes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8783 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/vardict.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    41836 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/vcoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3499 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/xmeta.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    61231 2024-05-22 17:48:25.000000 fstd2nc-0.20240401.2/fstd2nc/mixins/xycoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/fstd2nc/stdout.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-05-22 19:39:07.432969 fstd2nc-0.20240401.2/fstd2nc.egg-info/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-05-22 19:39:06.000000 fstd2nc-0.20240401.2/fstd2nc.egg-info/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1578 2024-05-22 19:39:07.432018 fstd2nc-0.20240401.2/fstd2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2024-05-22 19:39:06.000000 fstd2nc-0.20240401.2/fstd2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      289 2024-05-22 19:39:06.000000 fstd2nc-0.20240401.2/fstd2nc.egg-info/entry_points.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2024-05-22 19:39:07.432760 fstd2nc-0.20240401.2/fstd2nc.egg-info/requires.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2024-05-22 19:39:07.433006 fstd2nc-0.20240401.2/fstd2nc.egg-info/top_level.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.2/pyproject.toml
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1370 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.2/sample_meta.ini
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2024-05-22 19:39:07.440528 fstd2nc-0.20240401.2/setup.cfg
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2664 2024-05-15 20:02:51.000000 fstd2nc-0.20240401.2/setup.py
```

### Comparing `fstd2nc-0.20240401.1/.gitignore` & `fstd2nc-0.20240401.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/COPYING` & `fstd2nc-0.20240401.2/COPYING`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/COPYING.LESSER` & `fstd2nc-0.20240401.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/Changelog` & `fstd2nc-0.20240401.2/Changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Version 0.20240401.2 (May 22, 2024)
+	* More bug fixes for RSF support.
+	* Fixed auto-detect of legacy FST files in xarray.open_dataset.
+	  This was broken in 0.20240401.1 after adding RSF detection.
+	* Fixed crash when using --interp and --turbo features at the same
+	  time.
+	* Fixed --crop-to-smallest grid not working in some cases.
+	  decodeGrid was sometimes changing ig1/ig2/ig3 identifiers and causing
+	  a failure to find common grids.
+
 Version 0.20240401.1 (May 3, 2024)
 	* Fixed crash when importing fstd2nc.extra without having rpnpy or
 	  librmn in the environment.
 	* Some fixes for RSF support.  Detect more recent variants of header
 	  structures (e.g. for librmn 20.1.0-alpha3 snapshot).
 	* Fixed missing auto-detect for RSF in xarray interface.
 	* Fixed address overflow issue with CCC file interface, which was
```

### Comparing `fstd2nc-0.20240401.1/PKG-INFO` & `fstd2nc-0.20240401.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20240401.1
+Version: 0.20240401.2
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20240401.1/README.md` & `fstd2nc-0.20240401.2/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/README_fr.md` & `fstd2nc-0.20240401.2/README_fr.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/__init__.py` & `fstd2nc-0.20240401.2/cccbuffer/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/_xarray_hook.py` & `fstd2nc-0.20240401.2/cccbuffer/_xarray_hook.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/mixins/ccc.py` & `fstd2nc-0.20240401.2/cccbuffer/mixins/ccc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/mixins/char.py` & `fstd2nc-0.20240401.2/cccbuffer/mixins/char.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/mixins/grid.py` & `fstd2nc-0.20240401.2/cccbuffer/mixins/grid.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/mixins/levels.py` & `fstd2nc-0.20240401.2/cccbuffer/mixins/levels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/mixins/superlabels.py` & `fstd2nc-0.20240401.2/cccbuffer/mixins/superlabels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/cccbuffer/mixins/times.py` & `fstd2nc-0.20240401.2/cccbuffer/mixins/times.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/conda.recipe/README.md` & `fstd2nc-0.20240401.2/conda.recipe/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/conda.recipe/meta.yaml` & `fstd2nc-0.20240401.2/conda.recipe/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 package:
   name: fstd2nc
-  version: 0.20240401.1
+  version: 0.20240401.2
 
 
 requirements:
   build:
     - python
     - numpy  >1.15.3
     - netcdf4
```

### Comparing `fstd2nc-0.20240401.1/debian/control` & `fstd2nc-0.20240401.2/debian/control`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/debian/copyright` & `fstd2nc-0.20240401.2/debian/copyright`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/debian/rules` & `fstd2nc-0.20240401.2/debian/rules`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/__init__.py` & `fstd2nc-0.20240401.2/fstd2nc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ###############################################################################
 
 
 """
 Functionality for converting between FSTD and netCDF files.
 """
 
-__version__ = "0.20240401.1"
+__version__ = "0.20240401.2"
 
 
 # Check for bundled rpnpy package.
 # Fall back to this one if no standard rpnpy package available.
 try:
   # Importing the module will set up the appropriate search paths.
   import fstd2nc_deps
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc/__main__.py` & `fstd2nc-0.20240401.2/fstd2nc/__main__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/_xarray_hook.py` & `fstd2nc-0.20240401.2/fstd2nc/_xarray_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
       infiles = _expand_files(filename_or_obj)
       infiles = list(zip(*infiles))[1]
       if len(infiles) == 0: return False
       # Check first matching file.
       with open(infiles[0],'rb') as f:
         magic = f.read(24)
       # fstd98 in XDF container
-      if len(magic) >= 16 and magic[12:] == b'STDR':
+      if len(magic) >= 16 and magic[12:16] == b'STDR':
         return True
       # fst24 in RSF container (pre-release version?)
       elif len(magic) >= 24 and magic[16:24] == b'RSF0STDR':
         return True
       # fst24 in RSF container
       elif len(magic) >= 24 and magic[16:24] == b'RSF0STDF':
         return True
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc/extra.py` & `fstd2nc-0.20240401.2/fstd2nc/extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
       header_size = 18 + (data[0]&0x00ffff00)>>8
       header = data[4:4+18]
       xmeta = data[4+18:4+header_size]
       data = data[4+header_size:]
   else:
     data = data.view('>i4').astype('i4')
     header_size = 20    # FSTD, two aux keys need to be skipped.
-    header = data[:header_size]
+    header = data[:header_size-2] # Don't include aux keys in header output.
     xmeta = None
     data = data[header_size:]
   return header, xmeta, data
 
 
 def decode (data):
   '''
@@ -329,15 +329,15 @@
   # involved than a simple arithmetic operation.
   # NOTE: xtra1, xtra2, xtra3 not returned (not used, and take up space in the
   # header table).
 
   # Add RSF record info
   if rsf_info is not None:
     out['address'] = (rsf_info[:,0].astype(int)<<32) + rsf_info[:,1]
-    out['length'] = (rsf_info[:,2].astype(int)<<32) + rsf_info[:,2] - 16
+    out['length'] = (rsf_info[:,2].astype(int)<<32) + rsf_info[:,3] - 16
     # old 20.1.0 alpha2 version:
     if rsf_info.shape[1] == 6:
       out['meta_length'] = rsf_info[:,4].copy().view('H')[::2].copy()
     # some intermediate development version (?):
     elif rsf_info.shape[1] == 8:
       out['meta_length'] = rsf_info[:,6].copy().view('H')[::2].copy()
     # 20.1.0 alpha3 version:
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc/locale/Makefile` & `fstd2nc-0.20240401.2/fstd2nc/locale/Makefile`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/locale/README.md` & `fstd2nc-0.20240401.2/fstd2nc/locale/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo` & `fstd2nc-0.20240401.2/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fstd2nc\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-03 19:26+0000\n"
+"POT-Creation-Date: 2024-03-27 15:44+0000\n"
 "PO-Revision-Date: 2022-11-25 17:40+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ISO-8859-1\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -650,14 +650,17 @@
 
 msgid "an RPN standard file"
 msgstr "un fichier standard RPN"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" avec le mode %r"
 
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "impossible d'ouvrir '%s': %s"
+
 msgid "cannot have multiple subparser arguments"
 msgstr "impossible d'avoir plusiers arguments de sous-analyseur"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "impossible de fusionner les actions - deux groupes sont nommés %r"
 
 msgid "conflicting option string: %s"
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc/locale/fr_CA.po` & `fstd2nc-0.20240401.2/fstd2nc/locale/fr_CA.po`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/__init__.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/accum.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/accum.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/ascii.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/ascii.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/compat.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/compat.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/dates.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/dates.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/diaghacks.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/diaghacks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/ensembles.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/ensembles.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/extern.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/extern.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/filter.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/filter.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/fstd.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/fstd.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,16 +182,19 @@
     self._headers['dtype'] = np.empty(self._nrecs, dtype='|S2')
     self._headers['dtype'][:] = np.array(fast_dtype_fst2numpy(self._headers['datyp'],self._headers['nbits']))
     self._headers['selected'] = (self._headers['dltf']==0) & (self._headers['ismeta'] == False)
 
   # How to decode the data from a raw binary array.
   @classmethod
   def _decode (cls,data):
-    from fstd2nc.extra import decode
-    prm = cls._decode_headers(data[:72])
+    from fstd2nc.extra import _split_meta, decode
+    # Read a little extra past the header, since there may be a preamble
+    # (such as with RSF which leads with a "start of record" message).
+    meta, _, _ = _split_meta(data[:100])
+    prm = cls._decode_headers(meta[:72])
     nbits = int(prm['nbits'][0])
     datyp = int(prm['datyp'][0])
     dtype = dtype_fst2numpy(datyp, nbits)
     out = decode(data).view(dtype)
     return out
 
   # Shortcuts to header decoding functions.
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/gridhacks.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/gridhacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,20 +507,30 @@
     self._makevars()
     fstd2nc.stdout.streams = streams
     gids = self._gids
 
     # Find all available grids, group them by their projection parameters.
     # I.e., lump together all grids that only differ in their x/y extent.
     matches = dict()
-    for gid in np.unique(gids):
+    for gid, first_recid in zip(*np.unique(gids,return_index=True)):
       if gid<0: continue
       grid = rmn.decodeGrid(int(gid))
       # Skip supergrids.
       if grid['grtyp'] == 'U': continue
       key = (grid['ig1ref'],grid['ig2ref'],grid['ig3ref'],grid['ig4ref'])
+      # Fix up tags to match what's actually in the grid.
+      # For some reason sometimes decodeGrid gives different values for this?
+      grid = dict(grid)
+      grid['ig1'] = self._headers['ig1'][first_recid]
+      grid['ig2'] = self._headers['ig2'][first_recid]
+      grid['ig3'] = self._headers['ig3'][first_recid]
+      grid['tag1'] = self._headers['ig1'][first_recid]
+      grid['tag2'] = self._headers['ig2'][first_recid]
+      grid['tag3'] = self._headers['ig3'][first_recid]
+      # Add this grid to the list.
       matches.setdefault(key,[]).append(grid)
 
     # Find the smallest grid for each projection.
     smallest = dict()
     for key, grids in matches.items():
       shapes = [(len(grid['ax'].flatten()),len(grid['ay'].flatten())) for grid in grids]
       ind = shapes.index(min(shapes))
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/masks.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/masks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/mesh.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/misc.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/misc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/netcdf.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/netcdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,18 +449,18 @@
 
     # Now, do the actual transcribing of the data.
     # Read/write the data in the same order of records in the RPN file(s) to
     # improve performance.
     Bar = _ProgressBar if (progress is True and len(io) > 0) else _FakeBar
     bar = Bar(_("Saving netCDF file"), suffix="%(percent)d%% [%(myeta)s]", max=len(io)-1)
     if turbo:
-      from multiprocessing import Pool
+      from multiprocessing.pool import ThreadPool
       import numpy as np
       io = sorted(io)
-      with Pool() as p:
+      with ThreadPool() as p:
         raw = p.imap (self._read_record, (r for r,shape,v,ind in io))
         raw = bar.iter(raw)
         for (r,shape,v,ind), data in zip(io, raw):
           v[ind] = data.astype(v.dtype).reshape(shape)
         bar.finish()
     else:
       for r,shape,v,ind in bar.iter(sorted(io)):
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/pruneaxes.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/pruneaxes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/removestuff.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/removestuff.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/select.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/select.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/series.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/series.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/sfc_codes.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/sfc_codes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/vardict.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/vardict.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/vcoords.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/vcoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/xmeta.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/xmeta.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/mixins/xycoords.py` & `fstd2nc-0.20240401.2/fstd2nc/mixins/xycoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc/stdout.py` & `fstd2nc-0.20240401.2/fstd2nc/stdout.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/fstd2nc.egg-info/PKG-INFO` & `fstd2nc-0.20240401.2/fstd2nc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20240401.1
+Version: 0.20240401.2
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20240401.1/fstd2nc.egg-info/SOURCES.txt` & `fstd2nc-0.20240401.2/fstd2nc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/sample_meta.ini` & `fstd2nc-0.20240401.2/sample_meta.ini`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20240401.1/setup.py` & `fstd2nc-0.20240401.2/setup.py`

 * *Files identical despite different names*

