# Comparing `tmp/dea-tools-0.3.2.dev55.tar.gz` & `tmp/dea_tools-0.3.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dea-tools-0.3.2.dev55.tar", last modified: Tue Mar 19 04:52:58 2024, max compression
+gzip compressed data, was "dea_tools-0.3.3.dev9.tar", last modified: Wed May 22 06:50:43 2024, max compression
```

## Comparing `dea-tools-0.3.2.dev55.tar` & `dea_tools-0.3.3.dev9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:52:58.785496 dea-tools-0.3.2.dev55/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-03-19 04:52:58.785496 dea-tools-0.3.2.dev55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:52:58.781496 dea-tools-0.3.2.dev55/dea_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:52:58.781496 dea-tools-0.3.2.dev55/dea_tools/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32526 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20312 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/miningrehab.py
--rw-r--r--   0 runner    (1001) docker     (127)    11163 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (127)    20161 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    65692 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    76685 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)    55481 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (127)    40160 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/landcover.py
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    38380 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/pyfes_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    26490 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/waterbodies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/dea_tools/wetlands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:52:58.785496 dea-tools-0.3.2.dev55/dea_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-03-19 04:52:57.000000 dea-tools-0.3.2.dev55/dea_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-19 04:52:58.000000 dea-tools-0.3.2.dev55/dea_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 04:52:57.000000 dea-tools-0.3.2.dev55/dea_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-19 04:52:57.000000 dea-tools-0.3.2.dev55/dea_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 04:52:57.000000 dea-tools-0.3.2.dev55/dea_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:52:58.785496 dea-tools-0.3.2.dev55/gen/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.app.animations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.app.changefilmstrips.rst
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.app.crophealth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.app.deacoastlines.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.app.imageexport.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.app.miningrehab.rst
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.app.widgetconstructors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.bandindices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.bom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.classification.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.climate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.coastal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.dask.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.datahandling.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.landcover.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.plotting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.spatial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.temporal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/gen/dea_tools.waterbodies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 04:52:58.785496 dea-tools-0.3.2.dev55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-03-19 04:50:10.000000 dea-tools-0.3.2.dev55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:50:43.042806 dea_tools-0.3.3.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-22 06:50:43.042806 dea_tools-0.3.3.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:50:43.034806 dea_tools-0.3.3.dev9/dea_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:50:43.038806 dea_tools-0.3.3.dev9/dea_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32526 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20312 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/miningrehab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20161 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65692 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76685 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55481 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40160 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/landcover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38380 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/pyfes_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26490 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/waterbodies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/dea_tools/wetlands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:50:43.038806 dea_tools-0.3.3.dev9/dea_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-22 06:50:41.000000 dea_tools-0.3.3.dev9/dea_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-22 06:50:43.000000 dea_tools-0.3.3.dev9/dea_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:50:41.000000 dea_tools-0.3.3.dev9/dea_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-22 06:50:41.000000 dea_tools-0.3.3.dev9/dea_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 06:50:41.000000 dea_tools-0.3.3.dev9/dea_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:50:43.038806 dea_tools-0.3.3.dev9/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.app.animations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.app.changefilmstrips.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.app.crophealth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.app.deacoastlines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.app.imageexport.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.app.miningrehab.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.app.widgetconstructors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.bandindices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.bom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.climate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.coastal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.dask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.datahandling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.landcover.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.spatial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.temporal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/gen/dea_tools.waterbodies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:50:43.042806 dea_tools-0.3.3.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-22 06:47:46.000000 dea_tools-0.3.3.dev9/setup.py
```

### Comparing `dea-tools-0.3.2.dev55/LICENSE` & `dea_tools-0.3.3.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/PKG-INFO` & `dea_tools-0.3.3.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.3.2.dev55
+Version: 0.3.3.dev9
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.3.2.dev55/README.rst` & `dea_tools-0.3.3.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/app/animations.py` & `dea_tools-0.3.3.dev9/dea_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/app/changefilmstrips.py` & `dea_tools-0.3.3.dev9/dea_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/app/crophealth.py` & `dea_tools-0.3.3.dev9/dea_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/app/deacoastlines.py` & `dea_tools-0.3.3.dev9/dea_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/app/imageexport.py` & `dea_tools-0.3.3.dev9/dea_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/app/miningrehab.py` & `dea_tools-0.3.3.dev9/dea_tools/app/miningrehab.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/app/widgetconstructors.py` & `dea_tools-0.3.3.dev9/dea_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/bandindices.py` & `dea_tools-0.3.3.dev9/dea_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/bom.py` & `dea_tools-0.3.3.dev9/dea_tools/bom.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/classification.py` & `dea_tools-0.3.3.dev9/dea_tools/classification.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/climate.py` & `dea_tools-0.3.3.dev9/dea_tools/climate.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/coastal.py` & `dea_tools-0.3.3.dev9/dea_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/dask.py` & `dea_tools-0.3.3.dev9/dea_tools/dask.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/datahandling.py` & `dea_tools-0.3.3.dev9/dea_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/landcover.py` & `dea_tools-0.3.3.dev9/dea_tools/landcover.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/maps.py` & `dea_tools-0.3.3.dev9/dea_tools/maps.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/plotting.py` & `dea_tools-0.3.3.dev9/dea_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/pyfes_model.py` & `dea_tools-0.3.3.dev9/dea_tools/pyfes_model.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/spatial.py` & `dea_tools-0.3.3.dev9/dea_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/temporal.py` & `dea_tools-0.3.3.dev9/dea_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/validation.py` & `dea_tools-0.3.3.dev9/dea_tools/validation.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/waterbodies.py` & `dea_tools-0.3.3.dev9/dea_tools/waterbodies.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools/wetlands.py` & `dea_tools-0.3.3.dev9/dea_tools/wetlands.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/dea_tools.egg-info/PKG-INFO` & `dea_tools-0.3.3.dev9/dea_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.3.2.dev55
+Version: 0.3.3.dev9
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.3.2.dev55/dea_tools.egg-info/SOURCES.txt` & `dea_tools-0.3.3.dev9/dea_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dea-tools-0.3.2.dev55/index.rst` & `dea_tools-0.3.3.dev9/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
    dea_tools.coastal
    dea_tools.dask
    dea_tools.landcover
    dea_tools.plotting
    dea_tools.spatial
    dea_tools.temporal
    dea_tools.waterbodies
+   dea_tools.wetlands
    dea_tools.validation
    
 Apps and widgets
 -----------------
 
 ``dea_tools`` interactive app sub-packages can be accessed through ``dea_tools.app``.
```

### Comparing `dea-tools-0.3.2.dev55/setup.py` & `dea_tools-0.3.3.dev9/setup.py`

 * *Files identical despite different names*

