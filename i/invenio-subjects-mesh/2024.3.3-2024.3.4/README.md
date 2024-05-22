# Comparing `tmp/invenio-subjects-mesh-2024.3.3.tar.gz` & `tmp/invenio_subjects_mesh-2024.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-subjects-mesh-2024.3.3.tar", last modified: Thu Mar 21 19:35:30 2024, max compression
+gzip compressed data, was "invenio_subjects_mesh-2024.3.4.tar", last modified: Wed May 22 20:54:20 2024, max compression
```

## Comparing `invenio-subjects-mesh-2024.3.3.tar` & `invenio_subjects_mesh-2024.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:35:30.361479 invenio-subjects-mesh-2024.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-03-21 19:35:30.361479 invenio-subjects-mesh-2024.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:35:30.297478 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:35:30.361479 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127) 53592529 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh/vocabularies/subjects_mesh.csv
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh/vocabularies/vocabularies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:35:30.361479 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-03-21 19:35:30.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-21 19:35:30.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 19:35:30.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 19:35:30.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-21 19:35:30.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 19:35:30.000000 invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 19:35:30.361479 invenio-subjects-mesh-2024.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:35:30.361479 invenio-subjects-mesh-2024.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-21 19:35:22.000000 invenio-subjects-mesh-2024.3.3/tests/test_invenio_subjects_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:20.941838 invenio_subjects_mesh-2024.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 20:54:20.941838 invenio_subjects_mesh-2024.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:20.873838 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:20.941838 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127) 53592529 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh/vocabularies/subjects_mesh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh/vocabularies/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:20.941838 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 20:54:20.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-22 20:54:20.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:54:20.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 20:54:20.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 20:54:20.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 20:54:20.000000 invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:54:20.941838 invenio_subjects_mesh-2024.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:20.941838 invenio_subjects_mesh-2024.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-22 20:54:16.000000 invenio_subjects_mesh-2024.3.4/tests/test_invenio_subjects_mesh.py
```

### Comparing `invenio-subjects-mesh-2024.3.3/LICENSE` & `invenio_subjects_mesh-2024.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-2024.3.3/MANIFEST.in` & `invenio_subjects_mesh-2024.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-2024.3.3/PKG-INFO` & `invenio_subjects_mesh-2024.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-subjects-mesh
-Version: 2024.3.3
+Version: 2024.3.4
 Summary: MeSH subject terms with qualifiers
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -37,15 +37,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: galter-subjects-utils<2.0,>=0.3.2
+Requires-Dist: galter-subjects-utils<2.0,>=0.4.2
 Provides-Extra: dev
 Requires-Dist: check-manifest>=0.49; extra == "dev"
 Requires-Dist: invoke<3.0,>=2.2; extra == "dev"
 Requires-Dist: pyyaml>=5.4.1; extra == "dev"
 Requires-Dist: pytest-invenio<3.0.0,>=2.1.1; extra == "dev"
 
 # invenio-subjects-mesh
```

### Comparing `invenio-subjects-mesh-2024.3.3/README.md` & `invenio_subjects_mesh-2024.3.4/README.md`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh/vocabularies/subjects_mesh.csv` & `invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh/vocabularies/subjects_mesh.csv`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/PKG-INFO` & `invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-subjects-mesh
-Version: 2024.3.3
+Version: 2024.3.4
 Summary: MeSH subject terms with qualifiers
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -37,15 +37,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: galter-subjects-utils<2.0,>=0.3.2
+Requires-Dist: galter-subjects-utils<2.0,>=0.4.2
 Provides-Extra: dev
 Requires-Dist: check-manifest>=0.49; extra == "dev"
 Requires-Dist: invoke<3.0,>=2.2; extra == "dev"
 Requires-Dist: pyyaml>=5.4.1; extra == "dev"
 Requires-Dist: pytest-invenio<3.0.0,>=2.1.1; extra == "dev"
 
 # invenio-subjects-mesh
```

### Comparing `invenio-subjects-mesh-2024.3.3/invenio_subjects_mesh.egg-info/SOURCES.txt` & `invenio_subjects_mesh-2024.3.4/invenio_subjects_mesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-subjects-mesh-2024.3.3/pyproject.toml` & `invenio_subjects_mesh-2024.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "galter-subjects-utils>=0.3.2,<2.0",
+    "galter-subjects-utils>=0.4.2,<2.0",
 ]
 description = "MeSH subject terms with qualifiers"
 dynamic = ["version"]
 keywords = ["invenio", "inveniordm", "subjects", "MeSH"]
 license = {file = "LICENSE"}
 name = "invenio-subjects-mesh"
 readme = "README.md"
```

### Comparing `invenio-subjects-mesh-2024.3.3/tests/test_invenio_subjects_mesh.py` & `invenio_subjects_mesh-2024.3.4/tests/test_invenio_subjects_mesh.py`

 * *Files identical despite different names*

