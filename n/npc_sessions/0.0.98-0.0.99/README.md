# Comparing `tmp/npc_sessions-0.0.98.tar.gz` & `tmp/npc_sessions-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc_sessions-0.0.98.tar", last modified: Thu Oct 12 22:37:10 2023, max compression
+gzip compressed data, was "npc_sessions-0.0.99.tar", last modified: Sat Oct 14 01:01:23 2023, max compression
```

## Comparing `npc_sessions-0.0.98.tar` & `npc_sessions-0.0.99.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.748435 npc_sessions-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-10-12 22:37:10.748435 npc_sessions-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-10-12 22:37:04.000000 npc_sessions-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 22:37:10.748435 npc_sessions-0.0.98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.740434 npc_sessions-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.740434 npc_sessions-0.0.98/src/npc_sessions/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.740434 npc_sessions-0.0.98/src/npc_sessions/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/notebooks/dynamic_routing_qc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.744434 npc_sessions-0.0.98/src/npc_sessions/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/spikes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7577 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/plots/video.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.744434 npc_sessions-0.0.98/src/npc_sessions/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/scripts/write_dataframes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/scripts/write_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    75426 2023-10-12 22:37:00.000000 npc_sessions-0.0.98/src/npc_sessions/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.744434 npc_sessions-0.0.98/src/npc_sessions/trials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.744434 npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/
--rw-r--r--   0 runner    (1001) docker     (127)    40820 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/DynamicRouting1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/OptoTagging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/RFMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/trials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/trials/property_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.748435 npc_sessions-0.0.98/src/npc_sessions/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/barcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/electrodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/mvr.py
--rw-r--r--   0 runner    (1001) docker     (127)    24964 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/openephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/running.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/settings_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/spikeinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    46301 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/stim.py
--rw-r--r--   0 runner    (1001) docker     (127)    58942 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/utils/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/src/npc_sessions/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.740434 npc_sessions-0.0.98/src/npc_sessions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-10-12 22:37:10.000000 npc_sessions-0.0.98/src/npc_sessions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-10-12 22:37:10.000000 npc_sessions-0.0.98/src/npc_sessions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 22:37:10.000000 npc_sessions-0.0.98/src/npc_sessions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-12 22:37:10.000000 npc_sessions-0.0.98/src/npc_sessions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-12 22:37:10.000000 npc_sessions-0.0.98/src/npc_sessions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-12 22:37:10.000000 npc_sessions-0.0.98/src/npc_sessions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:37:10.748435 npc_sessions-0.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2023-10-12 22:22:39.000000 npc_sessions-0.0.98/tests/test_task_trials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.354386 npc_sessions-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-10-14 01:01:23.354386 npc_sessions-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2023-10-14 01:01:18.000000 npc_sessions-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 01:01:23.354386 npc_sessions-0.0.99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.346386 npc_sessions-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.346386 npc_sessions-0.0.99/src/npc_sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2023-10-14 01:01:14.000000 npc_sessions-0.0.99/src/npc_sessions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.350386 npc_sessions-0.0.99/src/npc_sessions/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-14 01:01:13.000000 npc_sessions-0.0.99/src/npc_sessions/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/notebooks/dynamic_routing_qc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2023-10-14 01:01:14.000000 npc_sessions-0.0.99/src/npc_sessions/notebooks/qc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.350386 npc_sessions-0.0.99/src/npc_sessions/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/plots/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2023-10-14 01:01:13.000000 npc_sessions-0.0.99/src/npc_sessions/plots/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/plots/spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/plots/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/plots/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/plots/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.350386 npc_sessions-0.0.99/src/npc_sessions/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/scripts/write_dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/scripts/write_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75678 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.350386 npc_sessions-0.0.99/src/npc_sessions/trials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.350386 npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/
+-rw-r--r--   0 runner    (1001) docker     (127)    40820 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/DynamicRouting1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/OptoTagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/RFMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/trials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/trials/property_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.350386 npc_sessions-0.0.99/src/npc_sessions/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/barcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/electrodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10268 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/mvr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24964 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/openephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/settings_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/spikeinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46301 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/stim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58942 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/utils/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/src/npc_sessions/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.346386 npc_sessions-0.0.99/src/npc_sessions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-10-14 01:01:23.000000 npc_sessions-0.0.99/src/npc_sessions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-10-14 01:01:23.000000 npc_sessions-0.0.99/src/npc_sessions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 01:01:23.000000 npc_sessions-0.0.99/src/npc_sessions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-14 01:01:23.000000 npc_sessions-0.0.99/src/npc_sessions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-14 01:01:23.000000 npc_sessions-0.0.99/src/npc_sessions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-14 01:01:23.000000 npc_sessions-0.0.99/src/npc_sessions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 01:01:23.354386 npc_sessions-0.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2023-10-14 00:48:08.000000 npc_sessions-0.0.99/tests/test_task_trials.py
```

### Comparing `npc_sessions-0.0.98/PKG-INFO` & `npc_sessions-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc_sessions
-Version: 0.0.98
+Version: 0.0.99
 Summary: Tools and interfaces for working with behavior and epyhys sessions from the Mindscope Neuropixels team, in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>, Ethan McBride <ethan.mcbride@alleninstitute.org>, Corbett Bennett <corbettb@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_sessions
 Project-URL: Issues, https://github.com/AllenInstitute/npc_sessions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `npc_sessions-0.0.98/README.md` & `npc_sessions-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/pyproject.toml` & `npc_sessions-0.0.99/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "npc_sessions"
-version = "0.0.98"
+version = "0.0.99"
 description = "Tools and interfaces for working with behavior and epyhys sessions from the Mindscope Neuropixels team, in the cloud."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
     { name = "Arjun Sridhar", email = "arjun.sridhar@alleninstitute.org" },
     { name = "Ethan McBride", email = "ethan.mcbride@alleninstitute.org" },
     { name = "Corbett Bennett", email = "corbettb@alleninstitute.org" },
 ]
@@ -187,14 +187,15 @@
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
     "--doctest-modules",
     "--ignore-glob=*scripts*,*examples*",
     "--cov",
     "--cov-report=xml",
+    "--cov-config=pyproject.toml",
     "--doctest-glob=*README.md",
     "-x",
     "-n=auto",
 ]
 doctest_optionflags = [
     "NORMALIZE_WHITESPACE",
     "IGNORE_EXCEPTION_DETAIL",
```

### Comparing `npc_sessions-0.0.98/src/npc_sessions/notebooks/dynamic_routing_qc.ipynb` & `npc_sessions-0.0.99/src/npc_sessions/notebooks/dynamic_routing_qc.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994748263888888%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'import pprint\\n'), (3, '\\n')]}}, 1: {'source': "*

 * *            "{insert: [(0, '# get input arguments from environment variables:\\n'), (1, 'env = "*

 * *            'os.environ\\n\'), (2, "session_path_or_id = env.pop(\'NPC_SESSION_PATH_OR_ID\')\\n"), '*

 * *            '(3, \'session_kwargs = {\\n\'), (4, "    k.replace(\'NPC_SESSION_\', \'\').lower(): '*

 * *            'eval(v)\\n"), (5, \'    for k, v in env.items()\\n\'), (6, "    if '*

 * *            'k.startswith(\'NPC_SESSION […]*

```diff
@@ -4,26 +4,41 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib inline\n",
                 "import os\n",
+                "import pprint\n",
+                "\n",
                 "import npc_sessions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# get input arguments from environment variables:\n",
+                "env = os.environ\n",
+                "session_path_or_id = env.pop('NPC_SESSION_PATH_OR_ID')\n",
+                "session_kwargs = {\n",
+                "    k.replace('NPC_SESSION_', '').lower(): eval(v)\n",
+                "    for k, v in env.items()\n",
+                "    if k.startswith('NPC_SESSION_')\n",
+                "}\n",
+                "\n",
                 "session = npc_sessions.DynamicRoutingSession(\n",
-                "    os.environ['NPC_SESSION_ID']\n",
-                ")"
+                "    session_path_or_id,\n",
+                "    **session_kwargs,\n",
+                ")\n",
+                "\n",
+                "print(f\"input:\\n{session_path_or_id = }\")\n",
+                "pprint.pprint(session_kwargs)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## behavior"
```

### Comparing `npc_sessions-0.0.98/src/npc_sessions/plots/audio.py` & `npc_sessions-0.0.99/src/npc_sessions/plots/audio.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/plots/behavior.py` & `npc_sessions-0.0.99/src/npc_sessions/plots/behavior.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,48 +121,59 @@
 
 
 def plot_running(
     session: "npc_sessions.DynamicRoutingSession",
 ) -> matplotlib.figure.Figure:
     timeseries = session.processing["behavior"]["running_speed"]
     epochs: pd.DataFrame = session.epochs[:]
+    licks = session.processing["behavior"]["licks"]
     plt.style.use("seaborn-v0_8-notebook")
 
     fig, ax = plt.subplots()
 
     for _, epoch in epochs.iterrows():
         epoch_indices = (timeseries.timestamps >= epoch["start_time"]) & (
             timeseries.timestamps <= epoch["stop_time"]
         )
         if len(epoch_indices) > 0:
             ax.plot(
                 timeseries.timestamps[epoch_indices],
                 timeseries.data[epoch_indices],
                 linewidth=0.1,
-                alpha=0.8,
+                alpha=1,
                 color="k",
+                label="speed",
+                zorder=30,
             )
     k = 100 if "cm" in timeseries.unit else 1
     ymax = 0.8 * k
-    plot_utils.add_epoch_color_bars(ax, epochs, rotation=90, y=ymax, va="top")
     ax.set_ylim([-0.05 * k, ymax])
+    ax.vlines(
+        licks.timestamps,
+        *ax.get_ylim(),
+        color="lime",
+        linestyle="-",
+        linewidth=0.05,
+        zorder=10,
+    )
     ax.hlines(
         0,
         0,
         max(timeseries.timestamps),
         color="k",
         linestyle="--",
         linewidth=0.5,
-        zorder=0,
+        zorder=20,
     )
+    plot_utils.add_epoch_color_bars(ax, epochs, rotation=90, y=ymax, va="top")
     ax.margins(0)
     ax.set_frame_on(False)
     ax.set_ylabel(timeseries.unit)
     ax.set_xlabel(timeseries.timestamps_unit)
     title = timeseries.description
     if max(timeseries.data) > ax.get_ylim()[1]:
-        title += f"\ndata clipped: {round(max(timeseries.data)) = } {timeseries.unit} at {timeseries.timestamps[np.argmax(timeseries.data)]} {timeseries.timestamps_unit}"
+        title += f"\ndata clipped: {round(max(timeseries.data)) = } {timeseries.unit} at {timeseries.timestamps[np.argmax(timeseries.data)]:.0f} {timeseries.timestamps_unit}"
     ax.set_title(title, fontsize=8)
     fig.suptitle(session.id, fontsize=10)
     fig.set_size_inches(10, 4)
     fig.set_layout_engine("tight")
     return fig
```

### Comparing `npc_sessions-0.0.98/src/npc_sessions/plots/plot_utils.py` & `npc_sessions-0.0.99/src/npc_sessions/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/plots/spikes.py` & `npc_sessions-0.0.99/src/npc_sessions/plots/spikes.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/plots/sync.py` & `npc_sessions-0.0.99/src/npc_sessions/plots/sync.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/plots/timing.py` & `npc_sessions-0.0.99/src/npc_sessions/plots/timing.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/plots/video.py` & `npc_sessions-0.0.99/src/npc_sessions/plots/video.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/scripts/write_dataframes.py` & `npc_sessions-0.0.99/src/npc_sessions/scripts/write_dataframes.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/scripts/write_notebooks.py` & `npc_sessions-0.0.99/src/npc_sessions/scripts/write_notebooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         session = npc_sessions.DynamicRoutingSession(session, **session_kwargs)
 
     # pass session to run in notebook via env var
     if session.info:
         var = session.info.allen_path.as_posix()
     else:
         var = str(session.id)
-    os.environ["NPC_SESSION_ID"] = var
+    os.environ["NPC_SESSION_PATH_OR_ID"] = var
 
     new_name = session.id if not session.info else session.info.allen_path.stem
     logger.info(f"running {QC_NOTEBOOK.name} for {session.id}")
     subprocess.run(
         f"jupyter nbconvert --to notebook --execute {QC_NOTEBOOK} --allow-errors --output {new_name}",
         shell=True,
         check=True,
```

### Comparing `npc_sessions-0.0.98/src/npc_sessions/sessions.py` & `npc_sessions-0.0.99/src/npc_sessions/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1571,16 +1571,20 @@
             session_id=self.id,
             start_time=start_time,
             stop_time=stop_time,
             tags=tags,
             notes=None if not notes else f"includes invalid times: {'; '.join(notes)}",
         )
 
-    @property
+    @utils.cached_property
     def ephys_record_node_dirs(self) -> tuple[upath.UPath, ...]:
+        if (v := getattr(self, "_ephys_record_node_dirs", None)) is not None:
+            paths = tuple(utils.from_pathlike(path) for path in v)
+            assert all("Record Node" in path.name for path in paths)
+            return paths
         return tuple(
             p for p in self.raw_data_paths if re.match(r"^Record Node [0-9]+$", p.name)
         )
 
     @utils.cached_property
     def ephys_recording_dirs(self) -> tuple[upath.UPath, ...]:
         return tuple(
```

### Comparing `npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/DynamicRouting1.py` & `npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/DynamicRouting1.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/OptoTagging.py` & `npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/OptoTagging.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/RFMapping.py` & `npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/RFMapping.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/trials/TaskControl/__init__.py` & `npc_sessions-0.0.99/src/npc_sessions/trials/TaskControl/__init__.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/trials/__init__.py` & `npc_sessions-0.0.99/src/npc_sessions/trials/__init__.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/trials/property_dict.py` & `npc_sessions-0.0.99/src/npc_sessions/trials/property_dict.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/barcodes.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/barcodes.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/electrodes.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/electrodes.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/file_io.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/misc.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/misc.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/mvr.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/mvr.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/openephys.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/openephys.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/running.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/running.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/settings_xml.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/settings_xml.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/spikeinterface.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/spikeinterface.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/stim.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/stim.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/sync.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/sync.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/utils/units.py` & `npc_sessions-0.0.99/src/npc_sessions/utils/units.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions/widgets.py` & `npc_sessions-0.0.99/src/npc_sessions/widgets.py`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/src/npc_sessions.egg-info/PKG-INFO` & `npc_sessions-0.0.99/src/npc_sessions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-sessions
-Version: 0.0.98
+Version: 0.0.99
 Summary: Tools and interfaces for working with behavior and epyhys sessions from the Mindscope Neuropixels team, in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>, Ethan McBride <ethan.mcbride@alleninstitute.org>, Corbett Bennett <corbettb@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_sessions
 Project-URL: Issues, https://github.com/AllenInstitute/npc_sessions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `npc_sessions-0.0.98/src/npc_sessions.egg-info/SOURCES.txt` & `npc_sessions-0.0.99/src/npc_sessions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 src/npc_sessions/widgets.py
 src/npc_sessions.egg-info/PKG-INFO
 src/npc_sessions.egg-info/SOURCES.txt
 src/npc_sessions.egg-info/dependency_links.txt
 src/npc_sessions.egg-info/entry_points.txt
 src/npc_sessions.egg-info/requires.txt
 src/npc_sessions.egg-info/top_level.txt
+src/npc_sessions/notebooks/__init__.py
 src/npc_sessions/notebooks/dynamic_routing_qc.ipynb
+src/npc_sessions/notebooks/qc.py
 src/npc_sessions/plots/__init__.py
 src/npc_sessions/plots/audio.py
 src/npc_sessions/plots/behavior.py
 src/npc_sessions/plots/plot_utils.py
 src/npc_sessions/plots/spikes.py
 src/npc_sessions/plots/sync.py
 src/npc_sessions/plots/timing.py
```

### Comparing `npc_sessions-0.0.98/src/npc_sessions.egg-info/requires.txt` & `npc_sessions-0.0.99/src/npc_sessions.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `npc_sessions-0.0.98/tests/test_task_trials.py` & `npc_sessions-0.0.99/tests/test_task_trials.py`

 * *Files identical despite different names*

