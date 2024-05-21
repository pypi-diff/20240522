# Comparing `tmp/pygeoprocessing-2.4.3.tar.gz` & `tmp/pygeoprocessing-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pygeoprocessing/pygeoprocessing/dist/.tmp-8bdv2xy9/pygeoprocessing-2.4.3.tar", last modified: Wed Mar  6 21:41:30 2024, max compression
+gzip compressed data, was "pygeoprocessing-2.4.4.tar", last modified: Tue May 21 22:37:32 2024, max compression
```

## Comparing `pygeoprocessing-2.4.3.tar` & `pygeoprocessing-2.4.4.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/.github/workflows/auto-pr-from-master-into-releases.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/.github/workflows/build-py-dists.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    62433 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    65839 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/ci/bugfix-release-pr-body.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/environment-rtd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    24154 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/source/_static/pygeoprocessing_logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/source/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/docs/source/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing-docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/pygeoprocessing-docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/pygeoprocessing-docker/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    65839 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/pygeoprocessing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/FastFileIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   214040 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/geoprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    40923 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/geoprocessing_core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26497 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/multiprocessing/raster_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/routing/
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/routing/LRUCache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/routing/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)   225106 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/routing/routing.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    44561 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/routing/watershed.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/slurm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/src/pygeoprocessing/symbolic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:41:30.000000 pygeoprocessing-2.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   257683 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/tests/test_geoprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/tests/test_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)    61351 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/tests/test_slurm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16391 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/tests/test_watershed_delineation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/tox-libcompat.ini
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-06 21:41:18.000000 pygeoprocessing-2.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.038201 pygeoprocessing-2.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.018201 pygeoprocessing-2.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.022201 pygeoprocessing-2.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/.github/workflows/auto-pr-from-master-into-releases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/.github/workflows/build-py-dists.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    63120 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    66662 2024-05-21 22:37:32.038201 pygeoprocessing-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.022201 pygeoprocessing-2.4.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/ci/bugfix-release-pr-body.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.022201 pygeoprocessing-2.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/environment-rtd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.022201 pygeoprocessing-2.4.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.022201 pygeoprocessing-2.4.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    24154 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/source/_static/pygeoprocessing_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/source/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/docs/source/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.022201 pygeoprocessing-2.4.4/pygeoprocessing-docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/pygeoprocessing-docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/pygeoprocessing-docker/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.038201 pygeoprocessing-2.4.4/pygeoprocessing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    66662 2024-05-21 22:37:31.000000 pygeoprocessing-2.4.4/pygeoprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-21 22:37:32.000000 pygeoprocessing-2.4.4/pygeoprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:37:31.000000 pygeoprocessing-2.4.4/pygeoprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:37:31.000000 pygeoprocessing-2.4.4/pygeoprocessing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 22:37:31.000000 pygeoprocessing-2.4.4/pygeoprocessing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 22:37:31.000000 pygeoprocessing-2.4.4/pygeoprocessing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:37:32.038201 pygeoprocessing-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.018201 pygeoprocessing-2.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.030201 pygeoprocessing-2.4.4/src/pygeoprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/FastFileIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211728 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/geoprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1906320 2024-05-21 22:37:27.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/geoprocessing_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    40855 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/geoprocessing_core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.030201 pygeoprocessing-2.4.4/src/pygeoprocessing/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26497 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/multiprocessing/raster_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.038201 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/LRUCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3584489 2024-05-21 22:37:29.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/routing.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   225106 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/routing.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1162410 2024-05-21 22:37:30.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/watershed.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    44517 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/routing/watershed.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/slurm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/src/pygeoprocessing/symbolic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:37:32.038201 pygeoprocessing-2.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   257631 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/tests/test_geoprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/tests/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61351 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/tests/test_slurm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16391 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/tests/test_watershed_delineation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/tox-libcompat.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-21 22:37:19.000000 pygeoprocessing-2.4.4/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pygeoprocessing-2.4.3/.github/workflows/auto-pr-from-master-into-releases.yml` & `pygeoprocessing-2.4.4/.github/workflows/auto-pr-from-master-into-releases.yml`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/.github/workflows/build-py-dists.yml` & `pygeoprocessing-2.4.4/.github/workflows/build-py-dists.yml`

 * *Files 22% similar despite different names*

```diff
@@ -4,41 +4,39 @@
     build-wheels:
         name: Wheel
         runs-on: ${{ matrix.os }}
         strategy:
             fail-fast: false
             matrix:
                 os: [windows-latest, macos-latest]
-                python-version: [3.7, 3.8, 3.9, "3.10", "3.11", "3.12"]
-                python-arch: [x64]
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
             - uses: actions/checkout@v4
               with:
                   # Fetch all history so that setuptools_scm can build the correct version string.
                   fetch-depth: 0
 
             - name: Fetch git tags
               run: git fetch origin +refs/tags/*:refs/tags/*
 
-            - name: Set up python ${{ matrix.python-version }} ${{ matrix.python-arch }}
-              uses: actions/setup-python@v4
+            - name: Set up python ${{ matrix.python-version }}
+              uses: actions/setup-python@v5
               with:
                   python-version: ${{ matrix.python-version }}
-                  architecture: ${{ matrix.python-arch }}
 
             - name: Install dependencies
               run: python -m pip install build
 
             - name: Build wheel
               run: python -m build --wheel
 
             - uses: actions/upload-artifact@v1
               with:
-                  name: Wheel for ${{ matrix.os }} ${{ matrix.python-version }} ${{ matrix.python-arch }}
+                  name: Wheel for ${{ matrix.os }} ${{ matrix.python-version }}
                   path: dist
 
     build-sdist:
         name: Source Dist
         runs-on: ubuntu-latest
         steps:
             - uses: actions/checkout@v4
@@ -46,17 +44,17 @@
                   # Fetch all history so that setuptools_scm can build the correct version string.
                   fetch-depth: 0
 
             - name: Fetch git tags
               run: git fetch origin +refs/tags/*:refs/tags/*
 
             - name: Set up python
-              uses: actions/setup-python@v4
+              uses: actions/setup-python@v5
               with:
-                  python-version: 3.7
+                  python-version: 3.12
 
             - name: Install dependencies
               run: python -m pip install build
 
             - name: Build source distribution
               run: python -m build --sdist
```

### Comparing `pygeoprocessing-2.4.3/.github/workflows/pythonpackage.yml` & `pygeoprocessing-2.4.4/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/HISTORY.rst` & `pygeoprocessing-2.4.4/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Release History
 ===============
 
+2.4.4 (2024-05-21)
+------------------
+* Our github actions for building python distributions now use
+  `actions/setup-python@v5`, which uses node 20.
+  https://github.com/natcap/pygeoprocessing/issues/384
+* ``warp_raster`` and ``build_overviews`` no longer raise a ``ValueError`` if
+  called with an invalid resampling algorithm. We now fall back to the
+  underlying GDAL functions' error messages.
+  https://github.com/natcap/pygeoprocessing/issues/387
+* Updated to Cython 3.
+* Dropped support for Python 3.7.
 
 2.4.3 (2024-03-06)
 ------------------
 * Wheels for python 3.12 are now built during our github actions runs.
   https://github.com/natcap/pygeoprocessing/issues/381
 * ``get_gis_type`` can accept a path to a remote file, allowing the GDAL driver
   to open it if the driver supports the protocol.
@@ -23,14 +34,17 @@
   In addition, the created mask raster's path may be defined by the caller so
   that it persists across calls to ``align_and_resize_raster_stack``.
   https://github.com/natcap/pygeoprocessing/issues/366
 * Improved ``warp_raster`` to allow for a pre-defined mask raster to be
   provided instead of a vector.  If both are provided, the mask raster alone is
   used.  The new mask raster must have the same dimensions and geotransform as
   the output warped raster. https://github.com/natcap/pygeoprocessing/issues/366
+* Fixed a bug in ``zonal_statistics`` where the wrong number of disjoint
+  polygon sets were being reported in the logs.
+  https://github.com/natcap/pygeoprocessing/issues/368
 * Pygeoprocessing is now tested against python 3.12.
   https://github.com/natcap/pygeoprocessing/issues/355
 
 2.4.2 (2023-10-24)
 ------------------
 * Fixed an issue where MFD flow direction was producing many nodata holes given
   a large-enough DEM.  These nodata holes would then propagate to flow
```

### Comparing `pygeoprocessing-2.4.3/LICENSE.txt` & `pygeoprocessing-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/PKG-INFO` & `pygeoprocessing-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: pygeoprocessing
-Version: 2.4.3
+Version: 2.4.4
 Summary: PyGeoprocessing: Geoprocessing routines for GIS
 Home-page: https://github.com/natcap/pygeoprocessing
 Maintainer: James Douglass
 Maintainer-email: jdouglass@stanford.edu
 License: BSD
 Keywords: gis pygeoprocessing
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: GDAL>=3.0.4
+Requires-Dist: numpy>=1.10.1
+Requires-Dist: Rtree>=0.8.3
+Requires-Dist: scipy!=0.19.1,>=0.14.1
+Requires-Dist: Shapely>=1.6.4
+Requires-Dist: importlib_metadata
 
 .. default-role:: code
 
 About PyGeoprocessing
 =====================
 
 PyGeoprocessing is a Python/Cython based library that provides a set of
@@ -82,14 +87,25 @@
 =================
 
 API documentation is available at https://pygeoprocessing.readthedocs.io/en/latest/
 
 Release History
 ===============
 
+2.4.4 (2024-05-21)
+------------------
+* Our github actions for building python distributions now use
+  `actions/setup-python@v5`, which uses node 20.
+  https://github.com/natcap/pygeoprocessing/issues/384
+* ``warp_raster`` and ``build_overviews`` no longer raise a ``ValueError`` if
+  called with an invalid resampling algorithm. We now fall back to the
+  underlying GDAL functions' error messages.
+  https://github.com/natcap/pygeoprocessing/issues/387
+* Updated to Cython 3.
+* Dropped support for Python 3.7.
 
 2.4.3 (2024-03-06)
 ------------------
 * Wheels for python 3.12 are now built during our github actions runs.
   https://github.com/natcap/pygeoprocessing/issues/381
 * ``get_gis_type`` can accept a path to a remote file, allowing the GDAL driver
   to open it if the driver supports the protocol.
@@ -108,14 +124,17 @@
   In addition, the created mask raster's path may be defined by the caller so
   that it persists across calls to ``align_and_resize_raster_stack``.
   https://github.com/natcap/pygeoprocessing/issues/366
 * Improved ``warp_raster`` to allow for a pre-defined mask raster to be
   provided instead of a vector.  If both are provided, the mask raster alone is
   used.  The new mask raster must have the same dimensions and geotransform as
   the output warped raster. https://github.com/natcap/pygeoprocessing/issues/366
+* Fixed a bug in ``zonal_statistics`` where the wrong number of disjoint
+  polygon sets were being reported in the logs.
+  https://github.com/natcap/pygeoprocessing/issues/368
 * Pygeoprocessing is now tested against python 3.12.
   https://github.com/natcap/pygeoprocessing/issues/355
 
 2.4.2 (2023-10-24)
 ------------------
 * Fixed an issue where MFD flow direction was producing many nodata holes given
   a large-enough DEM.  These nodata holes would then propagate to flow
```

### Comparing `pygeoprocessing-2.4.3/README.rst` & `pygeoprocessing-2.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/ci/bugfix-release-pr-body.md` & `pygeoprocessing-2.4.4/ci/bugfix-release-pr-body.md`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/docs/Makefile` & `pygeoprocessing-2.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/docs/make.bat` & `pygeoprocessing-2.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/docs/source/_static/pygeoprocessing_logo.jpg` & `pygeoprocessing-2.4.4/docs/source/_static/pygeoprocessing_logo.jpg`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/docs/source/basic_usage.rst` & `pygeoprocessing-2.4.4/docs/source/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/docs/source/conf.py` & `pygeoprocessing-2.4.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/docs/source/index.rst` & `pygeoprocessing-2.4.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/docs/source/installing.rst` & `pygeoprocessing-2.4.4/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/pygeoprocessing-docker/Dockerfile` & `pygeoprocessing-2.4.4/pygeoprocessing-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/pygeoprocessing.egg-info/PKG-INFO` & `pygeoprocessing-2.4.4/pygeoprocessing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: pygeoprocessing
-Version: 2.4.3
+Version: 2.4.4
 Summary: PyGeoprocessing: Geoprocessing routines for GIS
 Home-page: https://github.com/natcap/pygeoprocessing
 Maintainer: James Douglass
 Maintainer-email: jdouglass@stanford.edu
 License: BSD
 Keywords: gis pygeoprocessing
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: GDAL>=3.0.4
+Requires-Dist: numpy>=1.10.1
+Requires-Dist: Rtree>=0.8.3
+Requires-Dist: scipy!=0.19.1,>=0.14.1
+Requires-Dist: Shapely>=1.6.4
+Requires-Dist: importlib_metadata
 
 .. default-role:: code
 
 About PyGeoprocessing
 =====================
 
 PyGeoprocessing is a Python/Cython based library that provides a set of
@@ -82,14 +87,25 @@
 =================
 
 API documentation is available at https://pygeoprocessing.readthedocs.io/en/latest/
 
 Release History
 ===============
 
+2.4.4 (2024-05-21)
+------------------
+* Our github actions for building python distributions now use
+  `actions/setup-python@v5`, which uses node 20.
+  https://github.com/natcap/pygeoprocessing/issues/384
+* ``warp_raster`` and ``build_overviews`` no longer raise a ``ValueError`` if
+  called with an invalid resampling algorithm. We now fall back to the
+  underlying GDAL functions' error messages.
+  https://github.com/natcap/pygeoprocessing/issues/387
+* Updated to Cython 3.
+* Dropped support for Python 3.7.
 
 2.4.3 (2024-03-06)
 ------------------
 * Wheels for python 3.12 are now built during our github actions runs.
   https://github.com/natcap/pygeoprocessing/issues/381
 * ``get_gis_type`` can accept a path to a remote file, allowing the GDAL driver
   to open it if the driver supports the protocol.
@@ -108,14 +124,17 @@
   In addition, the created mask raster's path may be defined by the caller so
   that it persists across calls to ``align_and_resize_raster_stack``.
   https://github.com/natcap/pygeoprocessing/issues/366
 * Improved ``warp_raster`` to allow for a pre-defined mask raster to be
   provided instead of a vector.  If both are provided, the mask raster alone is
   used.  The new mask raster must have the same dimensions and geotransform as
   the output warped raster. https://github.com/natcap/pygeoprocessing/issues/366
+* Fixed a bug in ``zonal_statistics`` where the wrong number of disjoint
+  polygon sets were being reported in the logs.
+  https://github.com/natcap/pygeoprocessing/issues/368
 * Pygeoprocessing is now tested against python 3.12.
   https://github.com/natcap/pygeoprocessing/issues/355
 
 2.4.2 (2023-10-24)
 ------------------
 * Fixed an issue where MFD flow direction was producing many nodata holes given
   a large-enough DEM.  These nodata holes would then propagate to flow
```

### Comparing `pygeoprocessing-2.4.3/pygeoprocessing.egg-info/SOURCES.txt` & `pygeoprocessing-2.4.4/pygeoprocessing.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -28,23 +28,26 @@
 pygeoprocessing.egg-info/dependency_links.txt
 pygeoprocessing.egg-info/not-zip-safe
 pygeoprocessing.egg-info/requires.txt
 pygeoprocessing.egg-info/top_level.txt
 src/pygeoprocessing/FastFileIterator.h
 src/pygeoprocessing/__init__.py
 src/pygeoprocessing/geoprocessing.py
+src/pygeoprocessing/geoprocessing_core.cpp
 src/pygeoprocessing/geoprocessing_core.pyx
 src/pygeoprocessing/kernels.py
 src/pygeoprocessing/slurm_utils.py
 src/pygeoprocessing/symbolic.py
 src/pygeoprocessing/multiprocessing/__init__.py
 src/pygeoprocessing/multiprocessing/raster_calculator.py
 src/pygeoprocessing/routing/LRUCache.h
 src/pygeoprocessing/routing/__init__.py
 src/pygeoprocessing/routing/helper_functions.py
+src/pygeoprocessing/routing/routing.cpp
 src/pygeoprocessing/routing/routing.pyx
+src/pygeoprocessing/routing/watershed.cpp
 src/pygeoprocessing/routing/watershed.pyx
 tests/test_geoprocessing.py
 tests/test_kernels.py
 tests/test_routing.py
 tests/test_slurm_utils.py
 tests/test_watershed_delineation.py
```

### Comparing `pygeoprocessing-2.4.3/pyproject.toml` & `pygeoprocessing-2.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # these are the minimum packages needed in order to execute the pygeoprocessing build.
 # Setuptools, wheel are from pep508.
 # NOTE: GDAL is *not* require here because the compiled cython module will
 # dynamically import GDAL via python's import system.  This behavior means
 # that we can provide a much easier build experience so long as GDAL is
 # available at runtime.
 requires = [
-    'setuptools', 'wheel', 'setuptools_scm', 'cython<3.0.0', 'oldest-supported-numpy'
+    'setuptools', 'wheel', 'setuptools_scm', 'cython>=3.0.0', 'oldest-supported-numpy'
 ]
 build-backend = "setuptools.build_meta"
 
 
 [tool.pytest.ini_options]
 # Raise warnings to exceptions.
 filterwarnings = ["error", "default::DeprecationWarning", "default::FutureWarning"]
```

### Comparing `pygeoprocessing-2.4.3/setup.py` & `pygeoprocessing-2.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """setup.py module for PyGeoprocessing."""
 import platform
 
+from Cython.Build import cythonize
 import numpy
 from setuptools import setup
 from setuptools.extension import Extension
 
 # Read in requirements.txt and populate the python readme with the non-comment
 # contents.
 _REQUIREMENTS = [
@@ -48,25 +49,24 @@
         'Intended Audience :: Developers',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft',
         'Operating System :: POSIX',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Scientific/Engineering :: GIS',
         'License :: OSI Approved :: BSD License'
     ],
-    ext_modules=[
+    ext_modules=cythonize([
         Extension(
             name="pygeoprocessing.routing.routing",
             sources=["src/pygeoprocessing/routing/routing.pyx"],
             include_dirs=[
                 numpy.get_include(),
                 'src/pygeoprocessing/routing'],
             extra_compile_args=compiler_and_linker_args,
@@ -88,9 +88,9 @@
             sources=[
                 'src/pygeoprocessing/geoprocessing_core.pyx'],
             include_dirs=[numpy.get_include()],
             extra_compile_args=compiler_and_linker_args,
             extra_link_args=compiler_and_linker_args,
             language="c++"
         ),
-    ]
+    ])
 )
```

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/FastFileIterator.h` & `pygeoprocessing-2.4.4/src/pygeoprocessing/FastFileIterator.h`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/__init__.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/geoprocessing.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/geoprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,63 +72,14 @@
 
 _VALID_GDAL_TYPES = (
     set([getattr(gdal, x) for x in dir(gdal.gdalconst) if 'GDT_' in x]))
 
 _LOGGING_PERIOD = 5.0  # min 5.0 seconds per update log message for the module
 _LARGEST_ITERBLOCK = 2**16  # largest block for iterblocks to read in cells
 
-_GDAL_WARP_ALGORITHMS = []
-for _warp_algo in (_attrname for _attrname in dir(gdalconst)
-                   if _attrname.startswith('GRA_')):
-    # In GDAL < 3.4, the options used were actually gdal.GRIORA_*
-    # instead of gdal.GRA_*, and gdal.WarpOptions would:
-    #   * return an integer for any gdal.GRIORA options it didn't recognize
-    #   * Return an abbreviated string (e.g. -rb instead of 'bilinear') for
-    #     several warp algorithms
-    # This behavior was changed in GDAL 3.4, where the correct name is
-    # returned in all cases.
-    #
-    # In GDAL < 3.4, an error would be logged if GDAL couldn't recognize the
-    # option.  Pushing a null error handler avoids this and cleans up the
-    # logging.
-    gdal.PushErrorHandler(lambda *args: None)
-    _options = []
-    # GDAL's python bindings only offer this one way of translating gdal.GRA_*
-    # options to their string names (but compatibility is limited in different
-    # GDAL versions, see notes above)
-    warp_opts = gdal.WarpOptions(
-        options=_options,  # SIDE EFFECT: Adds flags to this list.
-        resampleAlg=getattr(gdalconst, _warp_algo),  # use GRA_* name.
-        overviewLevel=None)  # Don't add overview parameters.
-    gdal.PopErrorHandler()
-
-    # _options is populated during the WarpOptions call above.
-    for _item in _options:
-        is_int = False
-        try:
-            int(_item)
-            is_int = True
-        except ValueError:
-            pass
-
-        if _item == '-r':
-            continue
-        elif (_item.startswith('-r') and len(_item) > 2) or is_int:
-            # (GDAL < 3.4) Translate shorthand params to name.
-            # (GDAL < 3.4) Translate unrecognized (int) codes to name.
-            _item = re.sub('^gra_', '', _warp_algo.lower())
-        _GDAL_WARP_ALGORITHMS.append(_item)
-
-_GDAL_WARP_ALGORITHMS = set(_GDAL_WARP_ALGORITHMS)
-_GDAL_WARP_ALGOS_FOR_HUMAN_EYES = "|".join(_GDAL_WARP_ALGORITHMS)
-LOGGER.debug(
-    'Detected warp algorithms: '
-    f'{_GDAL_WARP_ALGOS_FOR_HUMAN_EYES.replace("|", ", ")}')
-
-
 class TimedLoggingAdapter(logging.LoggerAdapter):
     """A logging adapter to restrict logging based on a timer.
 
     The objective is to have a ``logging.LOGGER``-like object that can be
     called multiple times in rapid successtion, but with log messages only
     propagating every X seconds.
 
@@ -1886,41 +1837,42 @@
         gdal.Rasterize(
             destNameOrDestDS=fid_raster_path,
             srcDS=target_vector,
             allTouched=False,
             attribute=fid_field_name,
             noData=fid_nodata,
             outputBounds=aligned_bbox,
-            xRes=abs(raster_info['pixel_size'][0]),  # resolution should always be positive
+            xRes=abs(raster_info['pixel_size'][0]),  # resolution must be > 0
             yRes=abs(raster_info['pixel_size'][1]),
             format='GTIFF',
             outputType=gdal.GDT_UInt16,
             creationOptions=DEFAULT_GTIFF_CREATION_TUPLE_OPTIONS[1],
             callback=_make_logger_callback(
                 f'rasterizing disjoint polygon set {i + 1} of '
-                f'{len(disjoint_fid_set)} set %.1f%% complete (%s)'),
+                f'{len(disjoint_fid_sets)} set %.1f%% complete (%s)'),
             where=(f'{fid_field_name} IN ({fid_set_str})'))
         fid_raster_paths.append(fid_raster_path)
 
     timed_logger = TimedLoggingAdapter(_LOGGING_PERIOD)
     # Calculate statistics for each raster and each feature
     # working block-wise through the rasters
     for i, (raster_path, band) in enumerate(target_raster_path_band_list):
         LOGGER.info('calculating stats on raster '
                     f'{i} of {len(target_raster_path_band_list)}')
         # fetch the block offsets before the raster is opened for writing
         offset_list = list(iterblocks((raster_path, band), offset_only=True))
         nodata = get_raster_info(raster_path)['nodata'][band - 1]
         data_source = gdal.OpenEx(raster_path, gdal.OF_RASTER)
         data_band = data_source.GetRasterBand(band)
-        found_fids = set()  # track FIDs that have been found on at least one pixel
+        found_fids = set()  # track FIDs found on at least one pixel
 
         for set_index, fid_raster_path in enumerate(fid_raster_paths):
             LOGGER.info(
-                f'disjoint polygon set {set_index} of {len(fid_raster_paths)}')
+                f'disjoint polygon set {set_index + 1} of '
+                f'{len(fid_raster_paths)}')
             fid_raster = gdal.OpenEx(fid_raster_path, gdal.OF_RASTER)
             fid_band = fid_raster.GetRasterBand(1)
 
             for offset_index, offset in enumerate(offset_list):
                 timed_logger.info(
                     "%.1f%% done calculating stats for polygon set %s on raster %s",
                     offset_index / len(offset_list) * 100, set_index, i)
@@ -2479,15 +2431,16 @@
 
     Args:
         base_raster_path (string): path to base raster.
         target_pixel_size (list/tuple): a two element sequence indicating
             the x and y pixel size in projected units.
         target_raster_path (string): the location of the resized and
             resampled raster.
-        resample_method (string): the resampling technique, one of,
+        resample_method (string): the resampling algorithm. Must be a valid
+            resampling algorithm for `gdal.WarpRaster`, one of:
             'rms | mode | sum | q1 | near | q3 | average | cubicspline |
             bilinear | max | med | min | cubic | lanczos'
         target_bb (sequence): if None, target bounding box is the same as the
             source bounding box.  Otherwise it's a sequence of float
             describing target bounding box in target coordinate system as
             [minx, miny, maxx, maxy].
         base_projection_wkt (string): if not None, interpret the projection of
@@ -2663,19 +2616,14 @@
     base_raster = gdal.OpenEx(base_raster_path, gdal.OF_RASTER)
 
     raster_creation_options = list(raster_driver_creation_tuple[1])
     _, type_creation_options = _numpy_to_gdal_type(
         base_raster_info['numpy_type'])
     raster_creation_options += type_creation_options
 
-    if resample_method.lower() not in _GDAL_WARP_ALGORITHMS:
-        raise ValueError(
-            f'Invalid resample method: "{resample_method}". '
-            f'Must be one of {_GDAL_WARP_ALGOS_FOR_HUMAN_EYES}')
-
     gdal.Warp(
         warped_raster_path, base_raster,
         format=raster_driver_creation_tuple[0],
         outputBounds=working_bb,
         xRes=abs(target_pixel_size[0]),
         yRes=abs(target_pixel_size[1]),
         resampleAlg=resample_method,
@@ -2792,15 +2740,15 @@
     raster = gdal.OpenEx(target_raster_path, gdal.GA_Update | gdal.OF_RASTER)
     gdal.PopErrorHandler()
     if raster is None:
         raise ValueError(
             "%s doesn't exist, but needed to rasterize." % target_raster_path)
 
     rasterize_callback = _make_logger_callback(
-        "RasterizeLayer %.1f%% complete %s")
+        "pygeoprocessing.rasterize RasterizeLayer %.1f%% complete %s")
 
     if burn_values is None:
         burn_values = []
     if option_list is None:
         option_list = []
 
     if not burn_values and not option_list:
@@ -4628,15 +4576,16 @@
     Args:
         raster_path (str): A path to a raster on disk for which overviews
             should be built.
         internal=False (bool): Whether to modify the raster when building
             overviews. In GeoTiffs, this builds internal overviews when
             ``internal=True``, and external overviews when ``internal=False``.
         resample_method='near' (str): The resample method to use when
-            building overviews.  Must be one of,
+            building overviews.  Must be a valid resampling method for
+            ``gdal.GDALDataset.BuildOverviews``, one of
             'rms | mode | sum | q1 | near | q3 | average | cubicspline |
             bilinear | max | med | min | cubic | lanczos'.
         overwrite=False (bool): Whether to overwrite existing overviews, if
             any exist.
         levels='auto' (sequence): A sequence of integer overview levels. If
             ``'auto'``, overview levels will be determined by using factors of
             2 until the overview's x and y dimensions are both less than 256.
@@ -4652,19 +4601,14 @@
         resolution::
 
             build_overviews(raster_path, levels=[2, 4, 8, 16])
 
     Returns:
         ``None``
     """
-    if resample_method.lower() not in _GDAL_WARP_ALGORITHMS:
-        raise ValueError(
-            f'Invalid overview resample method: "{resample_method}". '
-            f'Must be one of {_GDAL_WARP_ALGOS_FOR_HUMAN_EYES}')
-
     def overviews_progress(*args, **kwargs):
         pct_complete, name, other = args
         percent = round(pct_complete * 100, 2)
         if time.time() - overviews_progress.last_progress_report > 5.0:
             LOGGER.info(f"Overviews progress: {percent}%")
             overviews_progress.last_progress_report = time.time()
     overviews_progress.last_progress_report = time.time()
```

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/geoprocessing_core.pyx` & `pygeoprocessing-2.4.4/src/pygeoprocessing/geoprocessing_core.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# coding=UTF-8
-# distutils: language=c++
-# cython: language_level=3
 import logging
 import multiprocessing
 import os
 import pickle
 import shutil
 import sys
 import tempfile
```

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/kernels.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/kernels.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/multiprocessing/raster_calculator.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/multiprocessing/raster_calculator.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/routing/LRUCache.h` & `pygeoprocessing-2.4.4/src/pygeoprocessing/routing/LRUCache.h`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/routing/__init__.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/routing/helper_functions.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/routing/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/routing/routing.pyx` & `pygeoprocessing-2.4.4/src/pygeoprocessing/routing/routing.pyx`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/routing/watershed.pyx` & `pygeoprocessing-2.4.4/src/pygeoprocessing/routing/watershed.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=UTF-8
-# cython: language_level=3
 import logging
 import os
 import shutil
 import tempfile
 import time
 
 cimport cython
```

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/slurm_utils.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/slurm_utils.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/src/pygeoprocessing/symbolic.py` & `pygeoprocessing-2.4.4/src/pygeoprocessing/symbolic.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/tests/test_geoprocessing.py` & `pygeoprocessing-2.4.4/tests/test_geoprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1749,20 +1749,20 @@
         base_a_path = os.path.join(self.workspace_dir, 'base_a.tif')
         _array_to_raster(
             pixel_a_matrix, target_nodata, base_a_path)
 
         target_raster_path = os.path.join(self.workspace_dir, 'target_a.tif')
         base_a_raster_info = pygeoprocessing.get_raster_info(base_a_path)
 
-        with self.assertRaises(ValueError) as context:
+        with self.assertRaises(TypeError) as context:
             pygeoprocessing.warp_raster(
                 base_a_path, base_a_raster_info['pixel_size'],
                 target_raster_path, 'not_an_algorithm', n_threads=1)
 
-        self.assertIn('Invalid resample method', str(context.exception))
+        self.assertIn('GDALWarpAppOptions', str(context.exception))
 
     def test_warp_raster_unusual_pixel_size(self):
         """PGP.geoprocessing: warp on unusual pixel types and sizes."""
         pixel_a_matrix = numpy.ones((1, 1), numpy.byte)
         target_nodata = -1
         base_a_path = os.path.join(self.workspace_dir, 'base_a.tif')
         _array_to_raster(
@@ -5549,20 +5549,19 @@
             pygeoprocessing.build_overviews(raster_path)
         self.assertIn("Raster already has overviews", str(cm.exception))
 
         # Forcibly overwriting the overviews should work fine, though.
         pygeoprocessing.build_overviews(raster_path, overwrite=True)
 
         # Check that we can catch invalid resample methods
-        with self.assertRaises(ValueError) as cm:
+        with self.assertRaises(RuntimeError) as cm:
             pygeoprocessing.build_overviews(
                 raster_path, overwrite=True,
                 resample_method='invalid choice')
-        self.assertIn('Invalid overview resample method: "invalid choice"',
-                      str(cm.exception))
+        self.assertIn('Building overviews failed', str(cm.exception))
 
     def test_get_raster_info_overviews(self):
         """PGP: raster info about overviews."""
         array = numpy.ones((2000, 1000), dtype=numpy.byte)
         raster_path = os.path.join(self.workspace_dir, 'raster.tif')
         _array_to_raster(array, 255, raster_path)
         pygeoprocessing.build_overviews(
```

### Comparing `pygeoprocessing-2.4.3/tests/test_kernels.py` & `pygeoprocessing-2.4.4/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/tests/test_routing.py` & `pygeoprocessing-2.4.4/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/tests/test_slurm_utils.py` & `pygeoprocessing-2.4.4/tests/test_slurm_utils.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/tests/test_watershed_delineation.py` & `pygeoprocessing-2.4.4/tests/test_watershed_delineation.py`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/tox-libcompat.ini` & `pygeoprocessing-2.4.4/tox-libcompat.ini`

 * *Files identical despite different names*

### Comparing `pygeoprocessing-2.4.3/tox.ini` & `pygeoprocessing-2.4.4/tox.ini`

 * *Files identical despite different names*

