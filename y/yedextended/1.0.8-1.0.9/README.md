# Comparing `tmp/yedextended-1.0.8.tar.gz` & `tmp/yedextended-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yedextended-1.0.8.tar", last modified: Wed May  1 12:20:46 2024, max compression
+gzip compressed data, was "yedextended-1.0.9.tar", last modified: Wed May  1 12:49:04 2024, max compression
```

## Comparing `yedextended-1.0.8.tar` & `yedextended-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 12:20:36.000000 yedextended-1.0.8/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.545099 yedextended-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.549100 yedextended-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-01 12:20:36.000000 yedextended-1.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-01 12:20:36.000000 yedextended-1.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 12:20:36.000000 yedextended-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-01 12:20:36.000000 yedextended-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:20:46.553099 yedextended-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-01 12:20:36.000000 yedextended-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic-create-and-open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic-formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic_bulk_manage1.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-basic_bulk_manage2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-custom-properties-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-multilabels.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-round-robin_read_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-uml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/demo-url-description-groups-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/readme-1.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/readme-2.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/readme-3.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/test.graphml
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/yed_created_edges.graphml
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-01 12:20:36.000000 yedextended-1.0.8/examples/yed_modified_app_created.graphml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/images/
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/demo_multilabel.png
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/example-UML.png
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/example.png
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/excel_obj_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/excel_rel_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/graph.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/graph_from_excel_obj.gif
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-01 12:20:36.000000 yedextended-1.0.8/images/graph_from_excel_rel.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-01 12:20:36.000000 yedextended-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 12:20:36.000000 yedextended-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:20:46.553099 yedextended-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.549100 yedextended-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/src/yedextended/
--rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-05-01 12:20:36.000000 yedextended-1.0.8/src/yedextended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/src/yedextended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 12:20:46.000000 yedextended-1.0.8/src/yedextended.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-01 12:20:36.000000 yedextended-1.0.8/test_coverage.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:46.553099 yedextended-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:20:36.000000 yedextended-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-01 12:20:36.000000 yedextended-1.0.8/tests/test_yedextended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.388076 yedextended-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 12:48:58.000000 yedextended-1.0.9/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.380076 yedextended-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.380076 yedextended-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-01 12:48:58.000000 yedextended-1.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-01 12:48:58.000000 yedextended-1.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 12:48:58.000000 yedextended-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-01 12:48:58.000000 yedextended-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:49:04.388076 yedextended-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-01 12:48:58.000000 yedextended-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic-create-and-open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic-formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic_bulk_manage1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic_bulk_manage2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-custom-properties-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-multilabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-round-robin_read_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-uml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-url-description-groups-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/readme-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/readme-2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/readme-3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/test.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/yed_created_edges.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/yed_modified_app_created.graphml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/demo_multilabel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/example-UML.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/excel_obj_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/excel_rel_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/graph.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/graph_from_excel_obj.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/graph_from_excel_rel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-01 12:48:58.000000 yedextended-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 12:48:58.000000 yedextended-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:49:04.388076 yedextended-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.380076 yedextended-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/src/yedextended/
+-rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-05-01 12:48:58.000000 yedextended-1.0.9/src/yedextended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.388076 yedextended-1.0.9/src/yedextended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-01 12:48:58.000000 yedextended-1.0.9/test_coverage.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:58.000000 yedextended-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-01 12:48:58.000000 yedextended-1.0.9/tests/test_yedextended.py
```

### Comparing `yedextended-1.0.8/.github/workflows/ci.yml` & `yedextended-1.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/.github/workflows/python-publish.yml` & `yedextended-1.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/.gitignore` & `yedextended-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/LICENSE` & `yedextended-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/PKG-INFO` & `yedextended-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yedextended-1.0.8/README.md` & `yedextended-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/demo-basic-create-and-open.py` & `yedextended-1.0.9/examples/demo-basic-create-and-open.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/demo-basic-formatting.py` & `yedextended-1.0.9/examples/demo-basic-formatting.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/demo-custom-properties-nodes-edges.py` & `yedextended-1.0.9/examples/demo-custom-properties-nodes-edges.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/demo-multilabels.py` & `yedextended-1.0.9/examples/demo-multilabels.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/demo-uml.py` & `yedextended-1.0.9/examples/demo-uml.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/demo-url-description-groups-nodes-edges.py` & `yedextended-1.0.9/examples/demo-url-description-groups-nodes-edges.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/readme-3.py` & `yedextended-1.0.9/examples/readme-3.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/test.graphml` & `yedextended-1.0.9/examples/test.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/yed_created_edges.graphml` & `yedextended-1.0.9/examples/yed_created_edges.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/examples/yed_modified_app_created.graphml` & `yedextended-1.0.9/examples/yed_modified_app_created.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/demo_multilabel.png` & `yedextended-1.0.9/images/demo_multilabel.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/example-UML.png` & `yedextended-1.0.9/images/example-UML.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/example.png` & `yedextended-1.0.9/images/example.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/excel_obj_entry.gif` & `yedextended-1.0.9/images/excel_obj_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/excel_rel_entry.gif` & `yedextended-1.0.9/images/excel_rel_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/graph.gif` & `yedextended-1.0.9/images/graph.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/graph_from_excel_obj.gif` & `yedextended-1.0.9/images/graph_from_excel_obj.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/images/graph_from_excel_rel.gif` & `yedextended-1.0.9/images/graph_from_excel_rel.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/pyproject.toml` & `yedextended-1.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,19 @@
 
 # Performing test coverage statistics - primarily for README.md
 [tool.coverage]
 
 [tool.coverage.run]
 branch = true
 relative_files = true
+# https://coverage.readthedocs.io/en/7.5.0/source.html#source
+omit = [
+	# omit everything in /tests
+	"tests/*",
+]
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_also = [
 	# Don't complain about missing debug-only code:
 	"def __repr__",
 	"if self\\.debug",
```

### Comparing `yedextended-1.0.8/src/yedextended/__init__.py` & `yedextended-1.0.9/src/yedextended/__init__.py`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/src/yedextended.egg-info/PKG-INFO` & `yedextended-1.0.9/src/yedextended.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yedextended-1.0.8/src/yedextended.egg-info/SOURCES.txt` & `yedextended-1.0.9/src/yedextended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/test_coverage.svg` & `yedextended-1.0.9/test_coverage.svg`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.8/tests/test_yedextended.py` & `yedextended-1.0.9/tests/test_yedextended.py`

 * *Files identical despite different names*

