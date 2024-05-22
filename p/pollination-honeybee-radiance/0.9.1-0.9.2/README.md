# Comparing `tmp/pollination-honeybee-radiance-0.9.1.tar.gz` & `tmp/pollination-honeybee-radiance-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-honeybee-radiance-0.9.1.tar", last modified: Tue May 25 01:30:02 2021, max compression
+gzip compressed data, was "dist/pollination-honeybee-radiance-0.9.2.tar", last modified: Tue Jun  1 23:34:06 2021, max compression
```

## Comparing `pollination-honeybee-radiance-0.9.1.tar` & `pollination-honeybee-radiance-0.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/.dependabot/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/.dependabot/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      572 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (121)     2941 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/contrib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/edit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/octree.py
--rw-r--r--   0 runner    (1001) docker     (121)     7373 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/post_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/raytrace.py
--rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/sky.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/sun.py
--rw-r--r--   0 runner    (1001) docker     (121)     5197 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 01:30:02.000000 pollination-honeybee-radiance-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/coefficient_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/contrib_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/edit_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/grid_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/matrix_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/octree_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/post_process_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/raytrace_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/sky_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/sun_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2021-05-25 01:28:52.000000 pollination-honeybee-radiance-0.9.1/tests/translate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/.dependabot/
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/.dependabot/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2803 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5748 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2627 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2941 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/edit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/octree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7373 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3236 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/raytrace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/sky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/sun.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5197 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2078 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-01 23:34:06.000000 pollination-honeybee-radiance-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/coefficient_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/contrib_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/edit_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/grid_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/matrix_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/octree_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/post_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/raytrace_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/sky_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/sun_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2021-06-01 23:33:08.000000 pollination-honeybee-radiance-0.9.2/tests/translate_test.py
```

### Comparing `pollination-honeybee-radiance-0.9.1/.github/workflows/ci.yaml` & `pollination-honeybee-radiance-0.9.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/.github/workflows/tests.yaml` & `pollination-honeybee-radiance-0.9.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/LICENSE` & `pollination-honeybee-radiance-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/PKG-INFO` & `pollination-honeybee-radiance-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-radiance
-Version: 0.9.1
+Version: 0.9.2
 Summary: Honeybee Radiance plugin for Pollination.
 Home-page: https://github.com/pollination/pollination-honeybee-radiance
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_bugs/grasshopper_tabs/HB-Radiance.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
 Description: # Pollination Honeybee Radiance plugin.
         
         The honeybee-radiance plugin adds daylight simulation functions to Pollination.
         
         This plugin takes advantage of Ladybug Tools `honeybee-radiance` Python package CLI.
-        For more information see: [PyPI](https://pypi.org/project/honeybee-radiance/) and [GitHub](https://github.com/ladybug-tools/honeybee-radiance).
+        For more information see: [PyPI](https://pypi.org/project/honeybee-radiance/) and
+        [GitHub](https://github.com/ladybug-tools/honeybee-radiance).
         
         For running all the functionalities on your local machine you need to install
         [Radiance](https://www.radiance-online.org/)). You can download the latest official
         release of Radiance from
         [GitHub](https://github.com/LBNL-ETA/Radiance/releases/tag/012cb178).
         
         # Functions
```

### Comparing `pollination-honeybee-radiance-0.9.1/README.md` & `pollination-honeybee-radiance-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Pollination Honeybee Radiance plugin.
 
 The honeybee-radiance plugin adds daylight simulation functions to Pollination.
 
 This plugin takes advantage of Ladybug Tools `honeybee-radiance` Python package CLI.
-For more information see: [PyPI](https://pypi.org/project/honeybee-radiance/) and [GitHub](https://github.com/ladybug-tools/honeybee-radiance).
+For more information see: [PyPI](https://pypi.org/project/honeybee-radiance/) and
+[GitHub](https://github.com/ladybug-tools/honeybee-radiance).
 
 For running all the functionalities on your local machine you need to install
 [Radiance](https://www.radiance-online.org/)). You can download the latest official
 release of Radiance from
 [GitHub](https://github.com/LBNL-ETA/Radiance/releases/tag/012cb178).
 
 # Functions
```

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/__init__.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/__init__.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/coefficient.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/coefficient.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/contrib.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/contrib.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/edit.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/edit.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/grid.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/grid.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/matrix.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/matrix.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/octree.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/octree.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/post_process.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/post_process.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/raytrace.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/raytrace.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/sky.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/sky.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/sun.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/sun.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination/honeybee_radiance/translate.py` & `pollination-honeybee-radiance-0.9.2/pollination/honeybee_radiance/translate.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/PKG-INFO` & `pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-radiance
-Version: 0.9.1
+Version: 0.9.2
 Summary: Honeybee Radiance plugin for Pollination.
 Home-page: https://github.com/pollination/pollination-honeybee-radiance
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_bugs/grasshopper_tabs/HB-Radiance.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
 Description: # Pollination Honeybee Radiance plugin.
         
         The honeybee-radiance plugin adds daylight simulation functions to Pollination.
         
         This plugin takes advantage of Ladybug Tools `honeybee-radiance` Python package CLI.
-        For more information see: [PyPI](https://pypi.org/project/honeybee-radiance/) and [GitHub](https://github.com/ladybug-tools/honeybee-radiance).
+        For more information see: [PyPI](https://pypi.org/project/honeybee-radiance/) and
+        [GitHub](https://github.com/ladybug-tools/honeybee-radiance).
         
         For running all the functionalities on your local machine you need to install
         [Radiance](https://www.radiance-online.org/)). You can download the latest official
         release of Radiance from
         [GitHub](https://github.com/LBNL-ETA/Radiance/releases/tag/012cb178).
         
         # Functions
```

### Comparing `pollination-honeybee-radiance-0.9.1/pollination_honeybee_radiance.egg-info/SOURCES.txt` & `pollination-honeybee-radiance-0.9.2/pollination_honeybee_radiance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/setup.py` & `pollination-honeybee-radiance-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/tests/grid_test.py` & `pollination-honeybee-radiance-0.9.2/tests/grid_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/tests/post_process_test.py` & `pollination-honeybee-radiance-0.9.2/tests/post_process_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/tests/raytrace_test.py` & `pollination-honeybee-radiance-0.9.2/tests/raytrace_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/tests/sky_test.py` & `pollination-honeybee-radiance-0.9.2/tests/sky_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-0.9.1/tests/translate_test.py` & `pollination-honeybee-radiance-0.9.2/tests/translate_test.py`

 * *Files identical despite different names*

