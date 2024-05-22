# Comparing `tmp/invenio-subjects-mesh-lite-2024.3.4.tar.gz` & `tmp/invenio_subjects_mesh_lite-2024.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-subjects-mesh-lite-2024.3.4.tar", last modified: Thu Mar 21 19:31:41 2024, max compression
+gzip compressed data, was "invenio_subjects_mesh_lite-2024.3.5.tar", last modified: Wed May 22 20:51:48 2024, max compression
```

## Comparing `invenio-subjects-mesh-lite-2024.3.4.tar` & `invenio_subjects_mesh_lite-2024.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:31:41.499601 invenio-subjects-mesh-lite-2024.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-03-21 19:31:41.499601 invenio-subjects-mesh-lite-2024.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:31:41.495602 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:31:41.495602 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1871337 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite/vocabularies/subjects_mesh.csv
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite/vocabularies/vocabularies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:31:41.499601 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-03-21 19:31:41.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-21 19:31:41.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 19:31:41.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-21 19:31:41.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-21 19:31:41.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-21 19:31:41.000000 invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 19:31:41.499601 invenio-subjects-mesh-lite-2024.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:31:41.495602 invenio-subjects-mesh-lite-2024.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-21 19:30:35.000000 invenio-subjects-mesh-lite-2024.3.4/tests/test_invenio_subjects_mesh_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:51:48.410470 invenio_subjects_mesh_lite-2024.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-22 20:51:48.410470 invenio_subjects_mesh_lite-2024.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:51:48.406470 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:51:48.410470 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1871337 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite/vocabularies/subjects_mesh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite/vocabularies/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:51:48.410470 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-22 20:51:48.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-22 20:51:48.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:51:48.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 20:51:48.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 20:51:48.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 20:51:48.000000 invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:51:48.410470 invenio_subjects_mesh_lite-2024.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:51:48.410470 invenio_subjects_mesh_lite-2024.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-22 20:50:35.000000 invenio_subjects_mesh_lite-2024.3.5/tests/test_invenio_subjects_mesh_lite.py
```

### Comparing `invenio-subjects-mesh-lite-2024.3.4/LICENSE` & `invenio_subjects_mesh_lite-2024.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-lite-2024.3.4/MANIFEST.in` & `invenio_subjects_mesh_lite-2024.3.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-lite-2024.3.4/PKG-INFO` & `invenio_subjects_mesh_lite-2024.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-subjects-mesh-lite
-Version: 2024.3.4
+Version: 2024.3.5
 Summary: MeSH subject terms without qualifiers
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -37,15 +37,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: galter-subjects-utils<2.0,>=0.3.3
+Requires-Dist: galter-subjects-utils<2.0,>=0.4.2
 Provides-Extra: dev
 Requires-Dist: check-manifest>=0.49; extra == "dev"
 Requires-Dist: invoke<3.0,>=2.2; extra == "dev"
 Requires-Dist: pyyaml>=5.4.1; extra == "dev"
 Requires-Dist: pytest-invenio<3.0.0,>=2.1.1; extra == "dev"
 
 # invenio-subjects-mesh-lite
```

### Comparing `invenio-subjects-mesh-lite-2024.3.4/README.md` & `invenio_subjects_mesh_lite-2024.3.5/README.md`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite/vocabularies/subjects_mesh.csv` & `invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite/vocabularies/subjects_mesh.csv`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/PKG-INFO` & `invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-subjects-mesh-lite
-Version: 2024.3.4
+Version: 2024.3.5
 Summary: MeSH subject terms without qualifiers
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -37,15 +37,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: galter-subjects-utils<2.0,>=0.3.3
+Requires-Dist: galter-subjects-utils<2.0,>=0.4.2
 Provides-Extra: dev
 Requires-Dist: check-manifest>=0.49; extra == "dev"
 Requires-Dist: invoke<3.0,>=2.2; extra == "dev"
 Requires-Dist: pyyaml>=5.4.1; extra == "dev"
 Requires-Dist: pytest-invenio<3.0.0,>=2.1.1; extra == "dev"
 
 # invenio-subjects-mesh-lite
```

### Comparing `invenio-subjects-mesh-lite-2024.3.4/invenio_subjects_mesh_lite.egg-info/SOURCES.txt` & `invenio_subjects_mesh_lite-2024.3.5/invenio_subjects_mesh_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-lite-2024.3.4/pyproject.toml` & `invenio_subjects_mesh_lite-2024.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "galter-subjects-utils>=0.3.3,<2.0"
+    "galter-subjects-utils>=0.4.2,<2.0"
 ]
 description = "MeSH subject terms without qualifiers"
 keywords = ["invenio", "inveniordm", "subjects", "MeSH"]
 license = {file = "LICENSE"}
 name = "invenio-subjects-mesh-lite"
 readme = "README.md"
 requires-python = ">=3.8"
 urls = {Repository = "https://github.com/galterlibrary/invenio-subjects-mesh-lite"}
-version = "2024.3.4"
+version = "2024.3.5"
 
 [project.optional-dependencies]
 dev = [
     "check-manifest>=0.49",
     "invoke>=2.2,<3.0",
     "pyyaml>=5.4.1",
     "pytest-invenio>=2.1.1,<3.0.0",
```

### Comparing `invenio-subjects-mesh-lite-2024.3.4/tests/test_invenio_subjects_mesh_lite.py` & `invenio_subjects_mesh_lite-2024.3.5/tests/test_invenio_subjects_mesh_lite.py`

 * *Files identical despite different names*

