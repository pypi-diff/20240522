# Comparing `tmp/crash-mapping-tools-0.0.1.tar.gz` & `tmp/crash_mapping_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crash-mapping-tools-0.0.1.tar", last modified: Tue Oct  3 23:03:59 2023, max compression
+gzip compressed data, was "crash_mapping_tools-0.0.2.tar", last modified: Wed May 22 16:30:23 2024, max compression
```

## Comparing `crash-mapping-tools-0.0.1.tar` & `crash_mapping_tools-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2023-10-03 23:03:59.122102 crash-mapping-tools-0.0.1/
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)     1061 2023-10-02 22:51:11.000000 crash-mapping-tools-0.0.1/LICENSE
--rw-r--r--   0 teshelman  (1000) teshelman  (1000)     2110 2023-10-03 23:03:59.122102 crash-mapping-tools-0.0.1/PKG-INFO
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       43 2023-10-02 22:51:11.000000 crash-mapping-tools-0.0.1/README.md
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)     1471 2023-10-03 23:02:38.000000 crash-mapping-tools-0.0.1/pyproject.toml
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       38 2023-10-03 23:03:59.122102 crash-mapping-tools-0.0.1/setup.cfg
-drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2023-10-03 23:03:59.122102 crash-mapping-tools-0.0.1/src/
-drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2023-10-03 23:03:59.122102 crash-mapping-tools-0.0.1/src/crash_mapping_tools/
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       91 2023-10-03 22:08:00.000000 crash-mapping-tools-0.0.1/src/crash_mapping_tools/__init__.py
-drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2023-10-03 23:03:59.122102 crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/
--rw-r--r--   0 teshelman  (1000) teshelman  (1000)     2110 2023-10-03 23:03:59.000000 crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/PKG-INFO
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)      352 2023-10-03 23:03:59.000000 crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)        1 2023-10-03 23:03:59.000000 crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       52 2023-10-03 23:03:59.000000 crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/entry_points.txt
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)      166 2023-10-03 23:03:59.000000 crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/requires.txt
--rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       20 2023-10-03 23:03:59.000000 crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/top_level.txt
+drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2024-05-22 16:30:23.986451 crash_mapping_tools-0.0.2/
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)     1061 2023-10-02 22:51:11.000000 crash_mapping_tools-0.0.2/LICENSE
+-rw-r--r--   0 teshelman  (1000) teshelman  (1000)     2131 2024-05-22 16:30:23.986451 crash_mapping_tools-0.0.2/PKG-INFO
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       43 2023-10-02 22:51:11.000000 crash_mapping_tools-0.0.2/README.md
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)     1484 2024-05-22 16:28:31.000000 crash_mapping_tools-0.0.2/pyproject.toml
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       38 2024-05-22 16:30:23.986451 crash_mapping_tools-0.0.2/setup.cfg
+drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2024-05-22 16:30:23.986451 crash_mapping_tools-0.0.2/src/
+drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2024-05-22 16:30:23.986451 crash_mapping_tools-0.0.2/src/crash_mapping_tools/
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)    33399 2024-05-22 16:07:51.000000 crash_mapping_tools-0.0.2/src/crash_mapping_tools/__init__.py
+drwxrwxr-x   0 teshelman  (1000) teshelman  (1000)        0 2024-05-22 16:30:23.986451 crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/
+-rw-r--r--   0 teshelman  (1000) teshelman  (1000)     2131 2024-05-22 16:30:23.000000 crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)      352 2024-05-22 16:30:23.000000 crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)        1 2024-05-22 16:30:23.000000 crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       52 2024-05-22 16:30:23.000000 crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)      172 2024-05-22 16:30:23.000000 crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/requires.txt
+-rw-rw-r--   0 teshelman  (1000) teshelman  (1000)       20 2024-05-22 16:30:23.000000 crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/top_level.txt
```

### Comparing `crash-mapping-tools-0.0.1/LICENSE` & `crash_mapping_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crash-mapping-tools-0.0.1/PKG-INFO` & `crash_mapping_tools-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crash-mapping-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Standalone tools for processing crash data
 Author-email: Tyler Eshelman <teshelman@edac.unm.edu>, Hays Barrett <hbarrett@edac.unm.edu>, Eric Crozier <ecrozier@edac.unm.edu>
 License: MIT License
         
         Copyright (c) 2023 EDAC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,10 +39,11 @@
 Requires-Dist: pyproj>=3.0.1
 Requires-Dist: Fiona>=1.8.20
 Requires-Dist: scikit-learn>=0.24.2
 Requires-Dist: scipy>=1.5.4
 Requires-Dist: shapely>=1.7.1
 Requires-Dist: geojson>=2.5.0
 Requires-Dist: GDAL==3.4.3
+Requires-Dist: pysal
 
 # crash-mapping-tools
 Crash Mapping Tools
```

### Comparing `crash-mapping-tools-0.0.1/pyproject.toml` & `crash_mapping_tools-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crash-mapping-tools"
-version = "0.0.1"
+version = "0.0.2"
 readme = "README.md"
 authors = [
     { name = "Tyler Eshelman", email = "teshelman@edac.unm.edu" },
     { name = "Hays Barrett", email = "hbarrett@edac.unm.edu" },
     { name = "Eric Crozier", email = "ecrozier@edac.unm.edu" },
 ]
 description = "Standalone tools for processing crash data"
@@ -26,23 +26,24 @@
     'geopandas >= 0.9.0',
     'pyproj >= 3.0.1',
     'Fiona >= 1.8.20',
     'scikit-learn >= 0.24.2',
     'scipy >= 1.5.4',
     'shapely >= 1.7.1',
     'geojson >= 2.5.0',
-    'GDAL==3.4.3'
+    'GDAL==3.4.3',
+    'pysal'
 ]
 requires-python = ">=3.7"
 
 [project.scripts]
 realpython = "reader.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `crash-mapping-tools-0.0.1/src/crash_mapping_tools.egg-info/PKG-INFO` & `crash_mapping_tools-0.0.2/src/crash_mapping_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crash-mapping-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Standalone tools for processing crash data
 Author-email: Tyler Eshelman <teshelman@edac.unm.edu>, Hays Barrett <hbarrett@edac.unm.edu>, Eric Crozier <ecrozier@edac.unm.edu>
 License: MIT License
         
         Copyright (c) 2023 EDAC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,10 +39,11 @@
 Requires-Dist: pyproj>=3.0.1
 Requires-Dist: Fiona>=1.8.20
 Requires-Dist: scikit-learn>=0.24.2
 Requires-Dist: scipy>=1.5.4
 Requires-Dist: shapely>=1.7.1
 Requires-Dist: geojson>=2.5.0
 Requires-Dist: GDAL==3.4.3
+Requires-Dist: pysal
 
 # crash-mapping-tools
 Crash Mapping Tools
```

