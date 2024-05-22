# Comparing `tmp/ironflow-0.1.0.tar.gz` & `tmp/ironflow-0.post0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironflow-0.1.0.tar", last modified: Wed May 22 20:29:10 2024, max compression
+gzip compressed data, was "ironflow-0.post0.dev1.tar", last modified: Thu Nov 10 17:19:15 2022, max compression
```

## Comparing `ironflow-0.1.0.tar` & `ironflow-0.post0.dev1.tar`

### file list

```diff
@@ -1,78 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.379106 ironflow-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-22 20:29:07.000000 ironflow-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 20:29:07.000000 ironflow-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-22 20:29:10.379106 ironflow-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-05-22 20:29:07.000000 ironflow-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.367106 ironflow-0.1.0/ironflow/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-22 20:29:10.379106 ironflow-0.1.0/ironflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.367106 ironflow-0.1.0/ironflow/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/draws_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.371106 ironflow-0.1.0/ironflow/gui/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.371106 ironflow-0.1.0/ironflow/gui/workflows/boxes/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.371106 ironflow-0.1.0/ironflow/gui/workflows/boxes/node_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/node_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/node_interface/control.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/node_interface/input_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/node_interface/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/text_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/boxes/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.371106 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/gui/workflows/screen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.375106 ironflow-0.1.0/ironflow/model/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15379 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23222 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/otypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/port.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/model/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.375106 ironflow-0.1.0/ironflow/node_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/node_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.375106 ironflow-0.1.0/ironflow/node_tools/input_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/node_tools/input_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/node_tools/main_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.375106 ironflow-0.1.0/ironflow/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.375106 ironflow-0.1.0/ironflow/nodes/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/deprecated/basic_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/deprecated/built_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/deprecated/control_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/deprecated/flow_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    21853 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/deprecated/special_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    36145 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/pyiron_atomistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/nodes/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 20:29:07.000000 ironflow-0.1.0/ironflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.375106 ironflow-0.1.0/ironflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-22 20:29:10.000000 ironflow-0.1.0/ironflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-22 20:29:10.000000 ironflow-0.1.0/ironflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:29:10.000000 ironflow-0.1.0/ironflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 20:29:10.000000 ironflow-0.1.0/ironflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 20:29:10.000000 ironflow-0.1.0/ironflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-22 20:29:10.379106 ironflow-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-22 20:29:10.000000 ironflow-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:29:10.375106 ironflow-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 20:29:07.000000 ironflow-0.1.0/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-22 20:29:07.000000 ironflow-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.858988 ironflow-0.post0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2022-11-10 17:19:15.858988 ironflow-0.post0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6474 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.862988 ironflow-0.post0.dev1/ironflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2022-11-10 17:19:15.862988 ironflow-0.post0.dev1/ironflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.850988 ironflow-0.post0.dev1/ironflow/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/custom_nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.850988 ironflow-0.post0.dev1/ironflow/custom_nodes/input_widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/custom_nodes/input_widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.850988 ironflow-0.post0.dev1/ironflow/gui/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.854988 ironflow-0.post0.dev1/ironflow/gui/boxes/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.854988 ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6039 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/control.py
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/input_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3488 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/representation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3144 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3436 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/boxes/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.854988 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5590 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6488 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9088 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/flow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10037 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2563 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/ports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13291 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.858988 ironflow-0.post0.dev1/ironflow/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/model/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9619 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/model/node.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.858988 ironflow-0.post0.dev1/ironflow/nodes/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7179 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/built_in.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.858988 ironflow-0.post0.dev1/ironflow/nodes/pyiron/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/pyiron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19938 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/pyiron/atomistics_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.858988 ironflow-0.post0.dev1/ironflow/nodes/std/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6428 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/std/basic_operators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4909 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/std/control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21897 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/ironflow/nodes/std/special_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 17:19:15.850988 ironflow-0.post0.dev1/ironflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2022-11-10 17:19:15.000000 ironflow-0.post0.dev1/ironflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2022-11-10 17:19:15.000000 ironflow-0.post0.dev1/ironflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-10 17:19:15.000000 ironflow-0.post0.dev1/ironflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2022-11-10 17:19:15.000000 ironflow-0.post0.dev1/ironflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-10 17:19:15.000000 ironflow-0.post0.dev1/ironflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2022-11-10 17:19:15.858988 ironflow-0.post0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2022-11-10 17:19:15.000000 ironflow-0.post0.dev1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68611 2022-11-10 17:19:12.000000 ironflow-0.post0.dev1/versioneer.py
```

### Comparing `ironflow-0.1.0/LICENSE` & `ironflow-0.post0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/boxes/base.py` & `ironflow-0.post0.dev1/ironflow/gui/boxes/base.py`

 * *Files identical despite different names*

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/boxes/flow.py` & `ironflow-0.post0.dev1/ironflow/gui/boxes/flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,22 @@
 Widgets for interacting with the flow diagram.
 """
 
 from __future__ import annotations
 
 import ipywidgets as widgets
 
-from ironflow.gui.draws_widgets import DrawsWidgets, draws_widgets
+from ironflow.gui.boxes.base import Box
 
 
-class NodeSelector(DrawsWidgets):
-    main_widget_class = widgets.VBox
+class NodeSelector(Box):
+    box_class = widgets.VBox
 
-    def __new__(cls, nodes_dictionary, *args, **kwargs):
-        return super().__new__(cls, *args, **kwargs)
-
-    def __init__(self, nodes_dictionary, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, nodes_dictionary):
+        super().__init__()
         self._nodes_dictionary = nodes_dictionary
 
         self.modules_dropdown = widgets.Dropdown(
             options=self.module_options,
             value=list(self.module_options)[0],
             disabled=False,
             layout=widgets.Layout(width="130px"),
@@ -33,15 +30,15 @@
             options=self.nodes_options,
             value=list(self.nodes_options)[0],
             disabled=False,
         )
 
         self.modules_dropdown.observe(self.change_modules_dropdown, names="value")
 
-        self.widget.children = [self.modules_dropdown, self.node_selector]
+        self.box.children = [self.modules_dropdown, self.node_selector]
 
     def change_modules_dropdown(self, change: dict) -> None:
         self.node_selector.options = sorted(
             self._nodes_dictionary[self.modules_dropdown.value].keys()
         )
 
     @property
@@ -54,61 +51,45 @@
     def module_options(self) -> list[str]:
         return sorted(self._nodes_dictionary.keys())
 
     @property
     def nodes_options(self) -> list[str]:
         return sorted(self._nodes_dictionary[self.modules_dropdown.value].keys())
 
-    def select_module(self, module_name):
-        self.modules_dropdown.value = module_name
-
     def update(self, nodes_dictionary: dict) -> None:
         self._nodes_dictionary = nodes_dictionary
         self.modules_dropdown.options = self.module_options
-        self.node_selector.options = self.nodes_options
 
 
-class FlowBox(DrawsWidgets):
-    def __new__(cls, nodes_dictionary, *args, **kwargs):
-        return super().__new__(cls, *args, **kwargs)
+class FlowBox(Box):
+    box_class = widgets.HBox
 
-    def __init__(self, nodes_dictionary: dict, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, nodes_dictionary: dict):
+        super().__init__()
         self.node_selector = NodeSelector(nodes_dictionary=nodes_dictionary)
         self.script_tabs = widgets.Tab([])
 
-        self.node_selector.widget.layout.width = "15%"
+        self.node_selector.box.layout.width = "15%"
         self.script_tabs.layout.width = "85%"
 
-        self.widget.children = [self.node_selector.widget, self.script_tabs]
+        self.box.children = [self.node_selector.box, self.script_tabs]
+
+    def update_nodes(self, nodes_dictionary: dict):
+        self.node_selector.update(nodes_dictionary=nodes_dictionary)
 
     def update_tabs(
         self, outputs: list[widgets.Output], titles: list[str], active_index: int
     ):
-        self._outputs = outputs
-        self._titles = titles
-        self._active_index = active_index
-        self.draw()
-
-    @draws_widgets
-    def draw(self):
         self.script_tabs.selected_index = None
         # ^ To circumvent a bug where the index gets set to 0 on child changes
         # https://github.com/jupyter-widgets/ipywidgets/issues/2988
-        self.script_tabs.children = self._outputs
-        for i, title in enumerate(self._titles):
+        self.script_tabs.children = outputs
+        for i, title in enumerate(titles):
             self.script_tabs.set_title(i, title)
         self._add_new_script_tab()
-        self.script_tabs.selected_index = self._active_index
-
-    def update_nodes(self, nodes_dictionary: dict):
-        self.node_selector.update(nodes_dictionary=nodes_dictionary)
+        self.script_tabs.selected_index = active_index
 
     def _add_new_script_tab(self):
         self.script_tabs.children += (
             widgets.Output(layout={"border": "1px solid black"}),
         )
         self.script_tabs.set_title(len(self.script_tabs.children) - 1, "+")
-
-    def close(self):
-        self.node_selector.close()
-        super().close()
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/boxes/node_interface/input_widgets.py` & `ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/input_widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 from typing import TYPE_CHECKING
 
 import ipywidgets as widgets
 
 if TYPE_CHECKING:
     from ironflow.model.node import Node
-    from ironflow.gui.workflows.screen import WorkflowsGUI
+    from ironflow.gui.gui import GUI
 
 
 class SliderControl:
-    def __init__(self, screen: WorkflowsGUI, node: Node):
-        self.screen = screen
+    def __init__(self, gui: GUI, node: Node):
+        self.gui = gui
         self.node = node
         self.widget = widgets.FloatSlider(
             value=self.node.val, min=0, max=10, continuous_update=False
         )
 
         self.widget.observe(self.widget_change, names="value")
 
     def widget_change(self, change: dict) -> None:
         self.node.set_state({"val": change["new"]}, 0)
         self.node.update_event()
-        self.screen.redraw_active_flow_canvas()
+        self.gui.redraw_active_flow_canvas()
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/boxes/node_interface/representation.py` & `ironflow-0.post0.dev1/ironflow/gui/boxes/node_interface/representation.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,75 +8,49 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import ipywidgets as widgets
 from IPython.display import display
 
-from ironflow.gui.draws_widgets import DrawsWidgets, draws_widgets
+from ironflow.gui.boxes.node_interface.base import NodeInterfaceBase
 
 if TYPE_CHECKING:
-    from ironflow.gui.workflows.canvas_widgets import NodeWidget
+    from ironflow.gui.canvas_widgets import NodeWidget
 
 
-class NodePresenter(DrawsWidgets):
+class NodePresenter(NodeInterfaceBase):
     """Handles the display of nodes with a representation."""
 
-    main_widget_class = widgets.VBox
-
     def __init__(self):
         super().__init__()
-        self.node_widget = None
+        self._node_widget = None
         self._widgets = []
         self._toggles = []
 
-        self._toggle_box = widgets.HBox([], layout={"flex_flow": "row wrap"})
-        self._representation_box = widgets.VBox([], layout={"max_height": "325px"})
-
-        self._border = "1px solid black"
-        self.widget.children = [self._toggle_box, self._representation_box]
-        self.widget.layout.width = "100%"
-        self.widget.layout.border = ""
-
-    def draw_for_node_widget(self, node_widget: NodeWidget):
-        self.clear()
-        self.node_widget = node_widget
-        if node_widget is not None:
-            self.draw()
-
-    def update(self) -> None:
-        if (
-            self.node_widget is not None
-            and self.node_widget.node.representation_updated
-        ):
-            self.draw()
-
-    @draws_widgets
-    def draw(self):
-        representations_dict = self.node_widget.node.representations
-
-        if len(representations_dict) != len(self._widgets):
-            self._widgets = self._build_widgets(representations_dict)
-            self._toggles = self._build_toggles(representations_dict)
-
-        for toggle, widget, representation in zip(
-            self._toggles, self._widgets, representations_dict.values()
-        ):
-            widget.clear_output()
-            widget.layout.border = ""
-            if toggle.value:
-                widget.layout.border = self._border
-                with widget:
-                    display(representation)
-
-        self._toggle_box.children = self._toggles
-        self._representation_box.children = self._widgets
-
-        self.node_widget.node.representation_updated = False
-        return self.widget
+    @property
+    def node_widget(self) -> NodeWidget | None:
+        return self._node_widget
+
+    @node_widget.setter
+    def node_widget(self, new_node_widget: NodeWidget | None):
+        if self._node_widget is not None:
+            self.clear_output()
+            self._node_widget.represent_button.pressed = False
+            self._node_widget.represent_button.draw()  # Re-draw it as un-pressed
+
+        if new_node_widget is not None:
+            new_node_widget.node.representation_updated = True
+            self._node_widget = new_node_widget
+            self._widgets = self._build_widgets(new_node_widget.node.representations)
+            self._toggles = self._build_toggles(new_node_widget.node.representations)
+        else:
+            self._node_widget = None
+            self._widgets = []
+            self._toggles = []
 
     @staticmethod
     def _build_widgets(representations: dict) -> list[widgets.Output]:
         return [
             widgets.Output(layout={"border": "solid 1px gray"}) for _ in representations
         ]
 
@@ -88,22 +62,47 @@
             )
             toggle.observe(self._on_toggle)
             toggles.append(toggle)
         return toggles
 
     def _on_toggle(self, change: dict) -> None:
         if change["name"] == "value":
-            self.draw()
+            self._draw()
 
-    def clear(self):
-        if self.node_widget is not None:
-            self.node_widget.represent_button.pressed = False
-            self.node_widget.represent_button.draw()  # Re-draw it as un-pressed
-        self.node_widget = None
+    def _draw(self):
+        self.clear_output()
 
-        self._widgets = []
-        self._toggles = []
+        representations = []
+        for (toggle, widget, representation) in zip(
+            self._toggles, self._widgets, self.node_widget.node.representations.values()
+        ):
+            if toggle.value:
+                with widget:
+                    display(representation)
+                representations.append(widget)
+
+        with self.output:
+            display(
+                widgets.VBox(
+                    [
+                        widgets.HBox(self._toggles, layout={"flex_flow": "row wrap"}),
+                        *representations,
+                    ]
+                )
+            )
+
+    def draw(self) -> None:
+        if (
+            self.node_widget is not None
+            and self.node_widget.node.representation_updated
+        ):
+            self._draw()
+            self.node_widget.node.representation_updated = False
 
-        self.widget.layout.border = ""
-        self._toggle_box.children = []
-        self._representation_box.children = []
-        super().clear()
+    def clear_output(self) -> None:
+        for w in self._widgets:
+            w.clear_output()
+        super().clear_output()
+
+    def close(self) -> None:
+        self.node_widget = None
+        self.clear_output()
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/boxes/text_output.py` & `ironflow-0.post0.dev1/ironflow/gui/boxes/text_output.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,38 +6,42 @@
 """
 
 from __future__ import annotations
 
 import ipywidgets as widgets
 from IPython.display import display
 
-from ironflow.gui.draws_widgets import DrawsWidgets
+from ironflow.gui.boxes.base import Box
 
 
-class TextOut(DrawsWidgets):
-    main_widget_class = widgets.VBox
+class TextOut(Box):
+    box_class = widgets.VBox
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.widget.width = "100%"
-        self.widget.border = "1px solid black"
+    def __init__(self):
+        super().__init__()
         self._output = widgets.Output()
         self._button = widgets.Button(
             tooltip="Clear output",
             description="clear",
             layout={"width": "100px"},
         )
         self._button.on_click(self._click_button)
 
+    @property
+    def layout(self):
+        return widgets.Layout(
+            width="100%",
+            border="1px solid black",
+        )
+
     def clear(self):
-        self._output.clear_output()
-        self.widget.children = []
         super().clear()
+        self._output.clear_output()
 
     def _click_button(self, change: dict) -> None:
         self.clear()
 
     def print(self, msg: str):
         self._output.clear_output()
         with self._output:
             display(msg)
-        self.widget.children = [self._output, self._button]
+        self.box.children = [self._output, self._button]
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/boxes/toolbar.py` & `ironflow-0.post0.dev1/ironflow/gui/boxes/toolbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A place to collect all the UI buttons.
 """
 
 from __future__ import annotations
 
 import ipywidgets as widgets
 
-from ironflow.gui.draws_widgets import DrawsWidgets
+from ironflow.gui.boxes.base import Box
 
 
 class Buttons:
     def __init__(self):
         """Toolbar buttons, declared in the order they will appear."""
         layout = widgets.Layout(width="50px")
         # Icon source: https://fontawesome.com
@@ -68,21 +68,21 @@
         )
 
     def __iter__(self):
         """Iterates like a list based on order of attribute declaration"""
         return self.__dict__.values().__iter__()
 
 
-class Toolbar(DrawsWidgets):
-    main_widget_class = widgets.HBox
+class Toolbar(Box):
+    box_class = widgets.HBox
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
         alg_modes = ["data", "exec"]
         self.alg_mode_dropdown = widgets.Dropdown(
             options=alg_modes,
             value=alg_modes[0],
             disabled=False,
             layout=widgets.Layout(width="80px"),
         )
         self.buttons = Buttons()
-        self.widget.children = [self.alg_mode_dropdown, *self.buttons]
+        self.box.children = [self.alg_mode_dropdown, *self.buttons]
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/boxes/user_input.py` & `ironflow-0.post0.dev1/ironflow/gui/boxes/user_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,39 +7,38 @@
 
 from __future__ import annotations
 
 from typing import Any, Optional
 
 import ipywidgets as widgets
 
-from ironflow.gui.draws_widgets import DrawsWidgets
+from ironflow.gui.boxes.base import Box
 
 
-class UserInput(DrawsWidgets):
-    main_widget_class = widgets.HBox
+class UserInput(Box):
+    box_class = widgets.HBox
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
         self.input_field = widgets.Text(value="INIT VALUE", description="DESCRIPTION")
         self.decision_info = widgets.Label(value="INIT VALUE")
         button_layout = widgets.Layout(width="50px")
         self.ok_button = widgets.Button(
             tooltip="Confirm", icon="check", layout=button_layout
         )
         self._last_ok_callback = None
         self.cancel_button = widgets.Button(
             tooltip="Cancel", icon="ban", layout=button_layout
         )
         # Todo: Use xmark once this is available
-        self.cancel_button.on_click(self._click_clear)
+        self.cancel_button.on_click(self.close)
 
     def clear(self):
-        self._clear_callback()
-        self.widget.children = []
         super().clear()
+        self._clear_callback()
 
     @property
     def text(self):
         return self.input_field.value
 
     def wrap_callback(self, callback: callable) -> callable:
         def wrapped_callback(change: dict) -> None:
@@ -64,15 +63,15 @@
     def _open(
         self,
         widget: widgets.Widget,
         callback: callable,
         ok_tooltip: str,
         cancel_tooltip: str,
     ):
-        self.widget.children = [widget, self.ok_button, self.cancel_button]
+        self._box.children = [widget, self.ok_button, self.cancel_button]
         self.ok_button.tooltip = ok_tooltip
         self.cancel_button.tooltip = cancel_tooltip
         self._set_callback(callback)
 
     def open_text(
         self,
         description: str,
@@ -96,9 +95,9 @@
         callback: callable,
         ok_tooltip: str = "Confirm",
         cancel_tooltip: str = "Cancel",
     ):
         self.decision_info.value = description
         self._open(self.decision_info, callback, ok_tooltip, cancel_tooltip)
 
-    def _click_clear(self, change: None):
+    def close(self, change: None):
         self.clear()
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/base.py` & `ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Optional, Union
 
+from ipycanvas import Canvas
+
+from ironflow.gui.canvas_widgets.layouts import Layout
+
 Number = Union[int, float]
 if TYPE_CHECKING:
-    from ipycanvas import Canvas
-    from ironflow.gui.workflows.canvas_widgets.flow import FlowCanvas
-    from ironflow.gui.workflows.screen import WorkflowsGUI
-    from ironflow.model.flow import Flow
-    from ironflow.model.model import HasSession
-    from ironflow.gui.workflows.canvas_widgets.layouts import Layout
+    from ironflow.gui.gui import GUI
+    from ironflow.gui.canvas_widgets.flow import FlowCanvas
+    from ironflow.model import Flow
 
 
 class CanvasWidget(ABC):
     """
     Parent class for all "widgets" that exist inside the scope of the flow canvas.
     """
 
@@ -72,22 +73,18 @@
         return self.parent.y + self._y
 
     @property
     def canvas(self) -> Canvas:
         return self.parent.canvas
 
     @property
-    def gui(self) -> HasSession:
+    def gui(self) -> GUI:
         return self.parent.gui
 
     @property
-    def screen(self) -> WorkflowsGUI:
-        return self.parent.screen
-
-    @property
     def flow(self) -> Flow:
         return self.parent.flow
 
     @property
     def flow_canvas(self) -> FlowCanvas:
         return self.parent.flow_canvas
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/buttons.py` & `ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/buttons.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Optional
 
-from ironflow.model.port import NodeInput, NodeOutput
-from ironflow.gui.workflows.canvas_widgets.base import CanvasWidget, HideableWidget
-from ironflow.gui.workflows.canvas_widgets.layouts import ButtonLayout
+from ironflow.gui.canvas_widgets.base import CanvasWidget, HideableWidget
+from ironflow.gui.canvas_widgets.layouts import ButtonLayout
+from ironflow.model import NodeInput, NodeOutput
 
 if TYPE_CHECKING:
-    from ironflow.gui.workflows.canvas_widgets.base import Number
-    from ironflow.gui.workflows.canvas_widgets.nodes import NodeWidget
+    from ironflow.gui.canvas_widgets.base import Number
+    from ironflow.gui.canvas_widgets.nodes import NodeWidget
     from ironflow.model import NodePort
 
 
 class ButtonWidget(CanvasWidget, ABC):
     def __init__(
         self,
         x: Number,
@@ -45,15 +45,15 @@
         self.deselect()
         return last_selected_object
 
     def press(self):
         self.pressed = True
         self.on_pressed()
         # Ok, now here is a weird hack:
-        self.screen.update_node_control()
+        self.gui.update_node_control()
         # This way, if a button causes some change in node-state, it gets reflected in the node_controller,
         # e.g. if we `run` or `remove` some job, but a nodestream node is taking that job as input.
         # Performance and usability hits are minimal, but from a maintenance perspective it is super bad, confusing,
         # and hard to maintain, so it would be much nicer in the future to find a way to hook the node_controller right
         #  onto input updates on the nodes
 
     def unpress(self):
@@ -96,18 +96,18 @@
         layout: ButtonLayout,
         selected: bool = False,
         title="SHOW",
     ):
         super().__init__(x, y, parent, layout, selected, title=title)
 
     def on_pressed(self):
-        self.screen.open_node_presenter(self.parent)
+        self.gui.open_node_presenter(self.parent)
 
     def on_unpressed(self):
-        self.screen.close_node_presenter()
+        self.gui.close_node_presenter()
 
 
 class ExpandCollapseButtonWidget(ButtonWidget, HideableWidget, ABC):
     def __init__(
         self,
         x: Number,
         y: Number,
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/flow.py` & `ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 from time import time
 from typing import TYPE_CHECKING, Optional
 
 import ipywidgets as widgets
 from ipycanvas import Canvas, hold_canvas
 from IPython.display import display
 
-from ironflow.model.port import NodeInput, NodeOutput
-from ironflow.gui.workflows.canvas_widgets.base import CanvasWidget
-from ironflow.gui.workflows.canvas_widgets.layouts import NodeLayout
-from ironflow.gui.workflows.canvas_widgets.nodes import NodeWidget
-from ironflow.gui.workflows.canvas_widgets.ports import PortWidget
+from ironflow.gui.canvas_widgets.base import CanvasWidget
+from ironflow.gui.canvas_widgets.buttons import RepresentButtonWidget
+from ironflow.gui.canvas_widgets.layouts import NodeLayout
+from ironflow.gui.canvas_widgets.nodes import NodeWidget, ButtonNodeWidget
+from ironflow.gui.canvas_widgets.ports import PortWidget
 
 if TYPE_CHECKING:
+    from ironflow.gui.canvas_widgets.base import Number
     from ironflow.gui.gui import GUI
-    from ironflow.gui.workflows.canvas_widgets.base import Number
-    from ironflow.gui.workflows.screen import WorkflowsGUI
-    from ironflow.model.flow import Flow
+    from ironflow.model import Flow
     from ironflow.model.node import Node
 
 
 class FlowCanvas:
     """
     A canvas for representing a particular Ryven script, which is determined at instantiation by the currently active
     gui script.
@@ -44,17 +43,17 @@
     Keyboard behaviour: Todo
         - ESC: Deselect all.
         - Backspace/Delete:
             - If a node is selected, deletes it
             - If a port is selected, deletes all connections it is part of
     """
 
-    def __init__(self, screen: WorkflowsGUI, flow: Flow):
-        self.screen = screen
-        self.flow = flow
+    def __init__(self, gui: GUI, flow: Optional[Flow] = None):
+        self._gui = gui
+        self.flow = flow if flow is not None else gui.flow
 
         self._standard_size = (1800, 800)
         self._zoom_factors = [0.50, 0.75, 1.00, 1.25, 1.50, 1.75, 2.00]
         self._zoom_index = 2
         self._width, self._height = self._get_size()
 
         self._canvas_color = "black"  # "#584f4e"
@@ -86,27 +85,26 @@
         self._mouse_is_down = False
         self._last_mouse_down = time()
         self._double_click_speed = (
             0.25  # In seconds. Todo: Put this in a config somewhere
         )
 
         self._object_to_gui_dict = {}
-        self._highlighted_ports: list[PortWidget] = []
 
     @property
     def canvas(self):
         return self._canvas
 
     @property
-    def flow_canvas(self) -> FlowCanvas:
-        return self
+    def gui(self):
+        return self._gui
 
     @property
-    def gui(self) -> GUI:
-        return self.screen.gui
+    def flow_canvas(self) -> FlowCanvas:
+        return self
 
     @property
     def title(self) -> str:
         return self.flow.script.title
 
     def display(self):
         self.output.clear_output()
@@ -157,15 +155,15 @@
         sel_object = self.get_element_at_xy(x, y)
         last_object = self._last_selected_object
 
         if sel_object is None:
             if last_object is not None:
                 last_object.deselect()
             elif time_since_last_click < self._double_click_speed:
-                self.add_node(x, y, self.screen.new_node_class)
+                self.add_node(x, y, self.gui.new_node_class)
                 self._built_object_to_gui_dict()
         else:
             if (
                 sel_object == last_object
                 and time_since_last_click < self._double_click_speed
             ):
                 sel_object = sel_object.on_double_click()
@@ -189,30 +187,30 @@
         return [o for o in self.objects_to_draw if o.selected]
 
     def handle_mouse_move(self, x: Number, y: Number) -> None:
         if self._mouse_is_down:
             selected_objects = self.get_selected_objects()
             if len(selected_objects) > 0:
                 with hold_canvas(self._canvas):
-                    [o.set_x_y(x - self.x, y - self.y) for o in selected_objects]
+                    [o.set_x_y(x, y) for o in selected_objects]
                     self.redraw()
             else:
                 self.x += x - self._x_move_anchor
                 self.y += y - self._y_move_anchor
                 self._x_move_anchor = x
                 self._y_move_anchor = y
                 self.redraw()
 
     def redraw(self) -> None:
         with hold_canvas(self._canvas):
             self.canvas_restart()
             [o.draw() for o in self.objects_to_draw]
             for c in self.flow.connections:
                 self.draw_connection(c.inp, c.out)
-        self.screen.update_node_presenter()
+        self.gui.update_node_presenter()
 
     def load_node(self, x: Number, y: Number, node: Node) -> NodeWidget:
         layout = NodeLayout()
 
         if hasattr(node, "main_widget_class") and node.main_widget_class is not None:
             if isinstance(node.main_widget_class, str):
                 node_class = eval(node.main_widget_class)
@@ -249,63 +247,14 @@
         if zoom_index != self._zoom_index:
             self._zoom_index = zoom_index
             self._width, self._height = self._get_size()
             self._canvas.width = self._width
             self._canvas.height = self._height
             self.redraw()
         else:
-            self.screen.print("Zoom limit reached")
+            self.gui.print("Zoom limit reached")
 
     def zoom_in(self) -> None:
         self._zoom(max(self._zoom_index - 1, 0))
 
     def zoom_out(self) -> None:
         self._zoom(min(self._zoom_index + 1, len(self._zoom_factors) - 1))
-
-    def highlight_compatible_ports(self, selected: PortWidget):
-        if selected.port.otype is None:
-            return
-
-        compatible_port_widgets = self._get_port_widgets_ontologically_compatible_with(
-            selected.port
-        )
-
-        for port_widget in compatible_port_widgets:
-            port_widget.highlight()
-        self._highlighted_ports = compatible_port_widgets
-
-    def _get_port_widgets_ontologically_compatible_with(self, port):
-        if isinstance(port, NodeInput):
-            input_tree = port.otype.get_source_tree(
-                additional_requirements=port.get_downstream_requirements()
-            )
-            return [
-                subwidget
-                for subwidget in self._port_widgets
-                if isinstance(subwidget.port, NodeOutput)
-                and subwidget.port.all_connections_found_in(input_tree)
-            ]
-        elif isinstance(port, NodeOutput):
-            return [
-                subwidget
-                for subwidget in self._port_widgets
-                if subwidget.port.otype is not None  # Progressively expensive checks
-                and port.otype in subwidget.port.otype.get_sources()
-                and subwidget.port.workflow_tree_contains_connections_of(port)
-            ]
-        else:
-            raise TypeError(
-                f"Expected a {NodeInput} or {NodeOutput} but got {type(port)}"
-            )
-
-    @property
-    def _port_widgets(self):
-        return [
-            subwidget
-            for node_widget in self.objects_to_draw
-            for subwidget in node_widget.objects_to_draw
-            if isinstance(subwidget, PortWidget)
-        ]
-
-    def clear_port_highlighting(self):
-        for port_widget in self._highlighted_ports:
-            port_widget.dehighlight()
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/layouts.py` & `ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/layouts.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,43 +24,37 @@
     @property
     def font_string(self):
         return f"{self.font_size}px {self.font}"
 
 
 @dataclass
 class NodeLayout(Layout):
-    width: int = 240
+    width: int = 200
     height: int = 100
     font_size: int = 22
     title_box_height: int = 30
     updating_color: str = "red"
-    max_title_chars: int = 14
 
 
 @dataclass
 class PortLayout(Layout, ABC):
     width: int = 20
     height: int = 20
-    max_title_chars: int = 10
-    highlight_color = "white"
 
 
 @dataclass
 class DataPortLayout(PortLayout):
-    valid_color: str = "lightgreen"
-    valid_selected_color: str = "darkgreen"
-    invalid_color: str = "red"
-    invalid_selected_color: str = "darkred"
+    background_color: str = "lightgreen"
+    selected_color: str = "darkgreen"
 
 
 @dataclass
 class ExecPortLayout(PortLayout):
-    # Exec ports have no data, so are always valid
-    valid_color: str = "lightblue"
-    valid_selected_color: str = "darkblue"
+    background_color: str = "lightblue"
+    selected_color: str = "darkblue"
 
 
 @dataclass
 class ButtonLayout(Layout):
     font_size: int = 16
     width: int = 60
     height: int = 20
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/canvas_widgets/nodes.py` & `ironflow-0.post0.dev1/ironflow/gui/canvas_widgets/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 import numpy as np
 from ipycanvas import hold_canvas
 
-from ironflow.gui.workflows.canvas_widgets.base import CanvasWidget
-from ironflow.gui.workflows.canvas_widgets.buttons import (
+from ironflow.gui.canvas_widgets.base import CanvasWidget
+from ironflow.gui.canvas_widgets.buttons import (
     RepresentButtonWidget,
     ExpandButtonWidget,
     CollapseButtonWidget,
     ExecButtonWidget,
 )
-from ironflow.gui.workflows.canvas_widgets.layouts import (
+from ironflow.gui.canvas_widgets.layouts import (
     NodeLayout,
     DataPortLayout,
     ExecPortLayout,
     ButtonLayout,
 )
-from ironflow.gui.workflows.canvas_widgets.ports import PortWidget
+from ironflow.gui.canvas_widgets.ports import PortWidget
 
 if TYPE_CHECKING:
-    from ironflow.gui.workflows.canvas_widgets.flow import FlowCanvas
-    from ironflow.gui.workflows.canvas_widgets.base import Number
-    from ironflow.model.port import NodeInputBP, NodeOutputBP
+    from ironflow.gui.canvas_widgets.flow import FlowCanvas
+    from ironflow.gui.canvas_widgets.base import Number
+    from ironflow.model import NodeInputBP, NodeOutputBP
     from ironflow.model.node import Node
 
 
 class NodeWidget(CanvasWidget):
     """
     The main ipycanvas representation of a node. Has graphical elements for IO ports. Collapsable to save space.
 
@@ -133,21 +133,21 @@
         if last_selected_object == self:
             return self
         else:
             if last_selected_object is not None:
                 last_selected_object.deselect()
             self.select()
             try:
-                self.screen.open_node_control(self.node)
+                self.gui.open_node_control(self.node)
                 return self
             except Exception as e:
-                self.screen.print(
+                self.gui.print(
                     f"Failed to handle selection of {self} with exception {e}"
                 )
-                self.screen.close_node_control()
+                self.gui.close_node_control()
                 self.deselect()
                 return None
 
     def on_double_click(self) -> None:
         self.delete()
         return None
 
@@ -175,31 +175,29 @@
     def draw_title(self) -> None:
         self.canvas.fill_style = self.node.color
         self.canvas.fill_rect(self.x, self.y, self.width, self._title_box_height)
         self.canvas.font = self.layout.font_string
         self.canvas.fill_style = self.layout.font_color
         x = self.x + (self.width * 0.04)
         y = self.y + self._title_box_height - 8
-        self.canvas.fill_text(self.title[: self.layout.max_title_chars], x, y)
+        self.canvas.fill_text(self.title, x, y)
 
     def _add_ports(
         self,
         radius: Number,
         inputs: Optional[list[NodeInputBP]] = None,
         outputs: Optional[list[NodeOutputBP]] = None,
         border: Number = 1.4,
     ) -> None:
         if inputs is not None:
             x = radius * border
             data = inputs
-            title_alignment = "start"
         elif outputs is not None:
             x = self.width - radius * border
             data = outputs
-            title_alignment = "end"
         else:
             return
 
         n_ports = len(data)
         for i_port in range(n_ports):
             port = data[i_port]
             data_or_exec = port.type_
@@ -209,15 +207,14 @@
                     y=self._subwidget_y_locs[i_port],
                     parent=self,
                     layout=self.port_layouts[data_or_exec],
                     port=port,
                     hidden_x=x,
                     hidden_y=self._subwidget_y_locs[0],
                     radius=radius,
-                    title_alignment=title_alignment,
                 )
             )
             if data_or_exec == "exec" and inputs is not None:
                 button_layout = ButtonLayout()
                 self.add_widget(
                     ExecButtonWidget(
                         x=x + radius,
@@ -231,28 +228,28 @@
     def add_inputs(self) -> None:
         self._add_ports(radius=self.port_radius, inputs=self.inputs)
 
     def add_outputs(self) -> None:
         self._add_ports(radius=self.port_radius, outputs=self.outputs)
 
     def delete(self) -> None:
-        self.screen.ensure_node_not_presented(self)
-        self.screen.ensure_node_not_controlled(self.node)
+        self.gui.ensure_node_not_presented(self)
+        self.gui.ensure_node_not_controlled(self.node)
         for c in self.flow.connections[
             ::-1
         ]:  # Reverse to make sure we traverse whole thing even if we delete
             # Todo: Can we be more efficient than looping over all nodes?
             if (c.inp.node == self.node) or (c.out.node == self.node):
                 self.flow.remove_connection(c)
         self.flow.remove_node(self.node)
         self.parent.objects_to_draw.remove(self)
 
     def deselect(self) -> None:
         super().deselect()
-        self.screen.ensure_node_not_controlled(self.node)
+        self.gui.ensure_node_not_controlled(self.node)
 
     @property
     def port_widgets(self) -> list[PortWidget]:
         return [o for o in self.objects_to_draw if isinstance(o, PortWidget)]
 
     def expand_io(self):
         self._height = self._expanded_height
```

### Comparing `ironflow-0.1.0/ironflow/gui/workflows/screen.py` & `ironflow-0.post0.dev1/ironflow/gui/gui.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,247 +1,325 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
-An interface for doing the visual scripting
+Top-level objects for getting the front and back end (and various parts of the front end) to talk to each other.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional, Type
 
 import ipywidgets as widgets
+from IPython.display import HTML
 
-from ironflow.gui.draws_widgets import DrawsWidgets, draws_widgets
-from ironflow.gui.workflows.boxes.flow import FlowBox
-from ironflow.gui.workflows.boxes.node_interface.control import NodeController
-from ironflow.gui.workflows.boxes.node_interface.representation import NodePresenter
-from ironflow.gui.workflows.boxes.text_output import TextOut
-from ironflow.gui.workflows.boxes.toolbar import Toolbar
-from ironflow.gui.workflows.boxes.user_input import UserInput
-from ironflow.gui.workflows.canvas_widgets.flow import FlowCanvas
-from ironflow.utils import display_string
+from ironflow.gui.boxes import (
+    Toolbar,
+    NodeController,
+    NodePresenter,
+    TextOut,
+    UserInput,
+    FlowBox,
+)
+from ironflow.gui.canvas_widgets import FlowCanvas
+from ironflow.model.model import HasSession
 
 if TYPE_CHECKING:
-    from ironflow.gui.gui import GUI
-    from ironflow.gui.workflows.canvas_widgets.nodes import NodeWidget
-    from ironflow.model.flow import Flow
     from ironflow.model.node import Node
-    from ironflow.model.port import NodeInput, NodeOutput
+    from ironflow.gui.canvas_widgets.nodes import NodeWidget
 
+debug_view = widgets.Output(layout={"border": "1px solid black"})
 
-class WorkflowsGUI(DrawsWidgets):
-    main_widget_class = widgets.VBox
 
-    def __new__(cls, gui, *args, **kwargs):
-        return super().__new__(cls, *args, **kwargs)
-
-    def __init__(self, gui: GUI, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+class GUI(HasSession):
+    """
+    The main ironflow object, connecting a ryven backend with a jupyter-friendly ipywidgets+ipycanvas frontend.
+
+    Methods:
+        draw: Build the ipywidget to interact with.
+        register_user_node: Register with ironflow a new node from the current python process.
+    """
+
+    def __init__(
+        self,
+        session_title: str,
+        extra_nodes_packages: Optional[list] = None,
+        script_title: Optional[str] = None,
+    ):
+        """
+        Create a new gui instance.
+
+        Args:
+            session_title (str): Title of the session to use. Will look for a json file of the same name and try to
+                read it. If no such file exists, simply makes a new script instead.
+            extra_nodes_packages (list | None): an optional list of nodes to register at instantiation. List items can
+                be either a list of `ironflow.model.node.Node` subclasses, a module containing such subclasses, or a .py
+                file of a module containing such subclasses. In all cases only those subclasses with the name pattern
+                `*_Node` will be registered. (Default is None, don't register any extra nodes.)
+            script_title (str|None): Title for an initial script. (Default is None, which generates "script_0" if a
+                new script is needed on initialization, i.e. when existing session data cannot be read.)
+        """
+        super().__init__(
+            session_title=session_title, extra_nodes_packages=extra_nodes_packages
+        )
 
-        self.gui = gui
         self.flow_canvases = []
-
         self.toolbar = Toolbar()
         self.node_controller = NodeController(self)
         self.node_presenter = NodePresenter()
         self.text_out = TextOut()
         self.input = UserInput()
-        self.flow_box = FlowBox(self.gui.nodes_dictionary)
+        self.flow_box = FlowBox(self.nodes_dictionary)
 
-        self.toolbar.alg_mode_dropdown.observe(
-            self._change_alg_mode_dropdown, names="value"
-        )
-        self.toolbar.buttons.help_node.on_click(self._click_node_help)
-        self.toolbar.buttons.load.on_click(self._click_load)
-        self.toolbar.buttons.save.on_click(self._click_save)
-        self.toolbar.buttons.add_node.on_click(self._click_add_node)
-        self.toolbar.buttons.delete_node.on_click(self._click_delete_node)
-        self.toolbar.buttons.create_script.on_click(self._click_create_script)
-        self.toolbar.buttons.rename_script.on_click(self._click_rename_script)
-        self.toolbar.buttons.delete_script.on_click(self._click_delete_script)
-        self.toolbar.buttons.zero_location.on_click(self._click_zero_location)
-        self.toolbar.buttons.zoom_in.on_click(self._click_zoom_in)
-        self.toolbar.buttons.zoom_out.on_click(self._click_zoom_out)
-        self.flow_box.script_tabs.observe(self._change_script_tabs)
+        try:
+            self.load(f"{self.session_title}.json")
+            print(f"Loaded session data for {self.session_title}")
+        except FileNotFoundError:
+            print(
+                f"No session data found for {self.session_title}, making a new script."
+            )
+            self.create_script(script_title)
+        self.update_tabs()
 
-        self.widget.children = [
-            self.toolbar.widget,
-            self.input.widget,
-            self.flow_box.widget,
-            self.text_out.widget,
-            widgets.HBox([self.node_controller.widget, self.node_presenter.widget]),
-        ]
+    def create_script(
+        self,
+        title: Optional[str] = None,
+        create_default_logs: bool = True,
+        data: Optional[dict] = None,
+    ) -> None:
+        super().create_script(
+            title=title, create_default_logs=create_default_logs, data=data
+        )
+        self.flow_canvases.append(FlowCanvas(gui=self))
 
-    @property
-    def new_node_class(self):
-        return self.flow_box.node_selector.new_node_class
+    def delete_script(self) -> None:
+        self.flow_canvases.pop(self.active_script_index)
+        self.node_controller.close()
+        self.node_presenter.close()
+        super().delete_script()
 
     @property
     def flow_canvas(self):
-        return self.flow_canvases[self.gui.active_script_index]
+        return self.flow_canvases[self.active_script_index]
 
     @property
-    def selected_node(self) -> Node | None:
-        selected = self.flow_canvas.get_selected_objects()
-        return selected[0].node if len(selected) > 0 else None
-
-    def update_tabs(self):
-        self.flow_box.update_tabs(
-            outputs=[fc.output for fc in self.flow_canvases],
-            titles=[fc.title for fc in self.flow_canvases],
-            active_index=self.gui.active_script_index,
-        )
-        for fc in self.flow_canvases:
-            fc.display()
+    def new_node_class(self):
+        return self.flow_box.node_selector.new_node_class
 
-    @draws_widgets
-    def add_flow(self, flow: Flow):
-        self.flow_canvases.append(FlowCanvas(screen=self, flow=flow))
+    def serialize(self) -> dict:
+        data = super().serialize()
+        currently_active = self.active_script_index
+        for i_script, script in enumerate(self.session.scripts):
+            all_data = data["scripts"][i_script]["flow"]["nodes"]
+            self.active_script_index = i_script
+            for i, node_widget in enumerate(self.flow_canvas.objects_to_draw):
+                all_data[i]["pos x"] = node_widget.x
+                all_data[i]["pos y"] = node_widget.y
+        self.active_script_index = currently_active
+        return data
 
-    @draws_widgets
-    def load_from_data(self, data: dict):
+    def load_from_data(self, data: dict) -> None:
+        super().load_from_data(data)
         self.flow_canvases = []
-        for i_script, script in enumerate(self.gui.session.scripts):
-            flow_canvas = FlowCanvas(screen=self, flow=script.flow)
+        for i_script, script in enumerate(self.session.scripts):
+            flow_canvas = FlowCanvas(gui=self, flow=script.flow)
             all_data = data["scripts"][i_script]["flow"]["nodes"]
             for i_node, node in enumerate(script.flow.nodes):
                 flow_canvas.load_node(
                     all_data[i_node]["pos x"], all_data[i_node]["pos y"], node
                 )
             flow_canvas._built_object_to_gui_dict()
             flow_canvas.redraw()
             self.flow_canvases.append(flow_canvas)
 
+    def register_node(self, node_class: Type[Node], node_group: Optional[str] = None):
+        # Inherited __doc__ still applies just fine, all we do here is update a menu item afterwards.
+        super().register_node(node_class=node_class, node_group=node_group)
+        try:
+            self.flow_box.node_selector.update(self.nodes_dictionary)
+        except AttributeError:
+            pass  # It's not defined yet in the super().__init__ call, which is fine
+
+    def update_tabs(self):
+        self.flow_box.update_tabs(
+            outputs=[fc.output for fc in self.flow_canvases],
+            titles=[fc.title for fc in self.flow_canvases],
+            active_index=self.active_script_index,
+        )
+        for fc in self.flow_canvases:
+            fc.display()
+
     def open_node_control(self, node: Node) -> None:
         self.node_controller.draw_for_node(node)
 
     def update_node_control(self) -> None:
-        self.node_controller.update()
+        self.node_controller.draw()
 
     def close_node_control(self) -> None:
-        self.node_controller.clear()
+        self.node_controller.node = None
+        self.node_controller.clear_output()
 
     def ensure_node_not_controlled(self, node: Node) -> None:
         if self.node_controller.node == node:
-            self.node_controller.clear()
+            self.node_controller.draw_for_node(None)
 
     def open_node_presenter(self, node_widget: NodeWidget):
-        self.node_presenter.draw_for_node_widget(node_widget)
+        self.node_presenter.node_widget = node_widget
 
     def update_node_presenter(self):
-        self.node_presenter.update()
+        self.node_presenter.draw()
 
     def close_node_presenter(self):
-        self.node_presenter.clear()
+        self.node_presenter.close()
 
     def ensure_node_not_presented(self, node_widget: NodeWidget) -> None:
         if self.node_presenter.node_widget == node_widget:
-            self.node_presenter.clear()
+            self.node_presenter.node_widget = None
 
     def redraw_active_flow_canvas(self):
         self.flow_canvas.redraw()
 
     def print(self, msg: str):
         self.text_out.print(msg)
 
-    def update_nodes_selector(self, nodes_dictionary: dict):
-        self.flow_box.node_selector.update(nodes_dictionary)
+    @debug_view.capture(clear_output=True)
+    def draw(self) -> widgets.VBox:
+        """
+        Build the gui.
+
+        Returns:
+            ipywidgets.VBox: The gui.
+        """
 
-    def delete_flow(self, i: int):
-        self.flow_canvases.pop(i)
-        self.node_controller.close()
-        self.node_presenter.clear()
+        # Wire callbacks
+        self.toolbar.alg_mode_dropdown.observe(
+            self._change_alg_mode_dropdown, names="value"
+        )
+        self.toolbar.buttons.help_node.on_click(self._click_node_help)
+        self.toolbar.buttons.load.on_click(self._click_load)
+        self.toolbar.buttons.save.on_click(self._click_save)
+        self.toolbar.buttons.add_node.on_click(self._click_add_node)
+        self.toolbar.buttons.delete_node.on_click(self._click_delete_node)
+        self.toolbar.buttons.create_script.on_click(self._click_create_script)
+        self.toolbar.buttons.rename_script.on_click(self._click_rename_script)
+        self.toolbar.buttons.delete_script.on_click(self._click_delete_script)
+        self.toolbar.buttons.zero_location.on_click(self._click_zero_location)
+        self.toolbar.buttons.zoom_in.on_click(self._click_zoom_in)
+        self.toolbar.buttons.zoom_out.on_click(self._click_zoom_out)
+        self.flow_box.script_tabs.observe(self._change_script_tabs)
 
+        return widgets.VBox(
+            [
+                self.toolbar.box,
+                self.input.box,
+                self.flow_box.box,
+                self.text_out.box,
+                widgets.HBox([self.node_controller.box, self.node_presenter.box]),
+                debug_view,
+            ]
+        )
+
+    # Type hinting for unused `change` argument in callbacks taken from ipywidgets docs:
+    # https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Events.html#Traitlet-events
     def _change_alg_mode_dropdown(self, change: dict) -> None:
         # Current behaviour: Updates the flow mode for all scripts
         # Todo: Change only for the active script, and update the dropdown on tab (script) switching
-        for script in self.gui.session.scripts:
+        for script in self.session.scripts:
             script.flow.set_algorithm_mode(self.toolbar.alg_mode_dropdown.value)
 
     def _click_save(self, change: dict) -> None:
         self.input.open_text(
             "Save file",
             self._click_confirm_save,
-            self.gui.session_title,
+            self.session_title,
             description_tooltip="Save to file name (omit the file extension, .json)",
         )
         self.print("Choose a file name to save to (omit the file extension, .json)")
 
     def _click_confirm_save(self, change: dict) -> None:
         file_name = self.input.text
-        self.gui.save(f"{file_name}.json")
+        self.save(f"{file_name}.json")
         self.print(f"Session saved to {file_name}.json")
         self.input.clear()
 
     def _click_load(self, change: dict) -> None:
         self.input.open_text(
             "Load file",
             self._click_confirm_load,
-            self.gui.session_title,
+            self.session_title,
             description_tooltip="Load from file name (omit the file extension, .json).",
         )
         self.print("Choose a file name to load (omit the file extension, .json)")
 
     def _click_confirm_load(self, change: dict) -> None:
         file_name = self.input.text
-        self.gui.load(f"{file_name}.json")
+        self.load(f"{file_name}.json")
         self.update_tabs()
-        self.node_presenter.clear()
+        self.node_presenter.clear_output()
         self.print(f"Session loaded from {file_name}.json")
         self.input.clear()
 
     def _click_node_help(self, change: dict) -> None:
-        self.print(
-            display_string(
-                f"{self.new_node_class.__name__.replace('_Node', '')}:\n{self.new_node_class.__doc__}"
+        def _pretty_docstring(node_class):
+            """
+            If we just pass a string, `display` doesn't resolve newlines.
+            If we pass a `print`ed string, `display` also shows the `None` value returned by `print`
+            So we use this ugly hack.
+            """
+            string = (
+                f"{node_class.__name__.replace('_Node', '')}:\n{node_class.__doc__}"
+            )
+            return HTML(
+                string.replace("\n", "<br>")
+                .replace("\t", "&emsp;")
+                .replace(" ", "&nbsp;")
             )
-        )
+
+        self.print(_pretty_docstring(self.new_node_class))
 
     def _click_add_node(self, change: dict) -> None:
         self.flow_canvas.add_node(10, 10, self.new_node_class)
 
     def _click_delete_node(self, change: dict) -> None:
         self.flow_canvas.delete_selected()
 
     def _click_create_script(self, change: dict) -> None:
-        self.gui.create_script()
+        self.create_script()
         self.update_tabs()
 
     def _click_rename_script(self, change: dict) -> None:
         self.input.open_text(
             "New name",
             self._click_confirm_rename,
-            self.gui.script.title,
+            self.script.title,
             description_tooltip="New script name",
         )
         self.print("Choose a new name for the current script")
 
     def _click_confirm_rename(self, change: dict) -> None:
         new_name = self.input.text
-        old_name = self.gui.script.title
-        rename_success = self.gui.rename_script(new_name)
+        old_name = self.script.title
+        rename_success = self.rename_script(new_name)
         if rename_success:
-            self.flow_box.script_tabs.set_title(self.gui.active_script_index, new_name)
+            self.flow_box.script_tabs.set_title(self.active_script_index, new_name)
             self.print(f"Script '{old_name}' renamed '{new_name}'")
         else:
             self.print(
-                f"INVALID NAME: Failed to rename script '{self.gui.script.title}' to '{new_name}'."
+                f"INVALID NAME: Failed to rename script '{self.script.title}' to '{new_name}'."
             )
 
     def _click_delete_script(self, change: dict) -> None:
         self.input.open_bool(
-            f"Delete the entire script {self.gui.script.title}?",
+            f"Delete the entire script {self.script.title}?",
             self._click_confirm_delete_script,
         )
 
     def _click_confirm_delete_script(self, change: dict) -> None:
-        script_name = self.gui.script.title
-        self.delete_flow(self.gui.active_script_index)
-        self.gui.delete_script()
+        script_name = self.script.title
+        self.delete_script()
         self.update_tabs()
         self.print(f"Script {script_name} deleted")
 
     def _click_zero_location(self, change: dict) -> None:
         self.flow_canvas.x = 0
         self.flow_canvas.y = 0
         self.flow_canvas.redraw()
@@ -256,21 +334,12 @@
         self.input.clear()
         self.text_out.clear()
 
     def _change_script_tabs(self, change: dict):
         if change["name"] == "selected_index" and change["new"] is not None:
             self.input.clear()
             self.flow_canvas.deselect_all()
-            if self.flow_box.script_tabs.selected_index == self.gui.n_scripts:
-                self.gui.create_script()
+            if self.flow_box.script_tabs.selected_index == self.n_scripts:
+                self.create_script()
                 self.update_tabs()
             else:
-                self.gui.active_script_index = self.flow_box.script_tabs.selected_index
-
-    def close(self):
-        self.toolbar.close()
-        self.node_controller.close()
-        self.node_presenter.close()
-        self.text_out.close()
-        self.input.close()
-        self.flow_box.close()
-        super().close()
+                self.active_script_index = self.flow_box.script_tabs.selected_index
```

### Comparing `ironflow-0.1.0/ironflow/model/model.py` & `ironflow-0.post0.dev1/ironflow/model/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,51 +12,44 @@
 import types
 from abc import ABC
 from inspect import isclass
 from pathlib import Path
 from types import ModuleType
 from typing import Optional, Type
 
+from ryvencore import Session, Script, Flow
+
 from ironflow.model.node import Node
-from ironflow.model.port import NodeInput, NodeOutput
-from ironflow.model.session import Session
-from ironflow.model.flow import Flow
-from ironflow.model.script import Script
 
 
 class HasSession(ABC):
     """Mixin for an object which has a Ryven session as the underlying model"""
 
-    def __init__(
-        self,
-        session_title: str,
-        *args,
-        extra_nodes_packages: Optional[list] = None,
-        enable_ryven_log: bool = False,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
+    def __init__(self, session_title: str, extra_nodes_packages: Optional[list] = None):
         self._session = Session()
         self.session_title = session_title
         self._active_script_index = 0
 
-        if enable_ryven_log:
-            self.session.info_messenger().enable()
-
-        self.nodes_dictionary = {"recommended": {}}
-        from ironflow.nodes import array, plot, pyiron_atomistics, standard
+        self.nodes_dictionary = {}
+        from ironflow.nodes import built_in
+        from ironflow.nodes.pyiron import atomistics_nodes
+        from ironflow.nodes.std import (
+            basic_operators,
+            control_structures,
+            special_nodes,
+        )
 
         for module in [
-            array,
-            plot,
-            pyiron_atomistics,
-            standard,
+            built_in,
+            atomistics_nodes,
+            basic_operators,
+            control_structures,
+            special_nodes,
         ]:
             self.register_nodes_from_module(module)
-        self._starting_module = pyiron_atomistics.__name__.split(".")[-1]
 
         if extra_nodes_packages is not None:
             for package in extra_nodes_packages:
                 # Todo: Figure out how to allow node_group to be passed in in an elegant way here for each package
                 self.register_nodes(package)
 
     @property
@@ -161,15 +154,15 @@
                 update. Already-placed nodes are still instances of the old class and need to be deleted.
 
         Note: You can save the graph as normal, but new gui instances will need to register the same custom nodes before
             loading the saved graph is possible.
 
         Example:
             >>> from ironflow import GUI
-            >>> from ironflow.node_tools import Node, NodeInputBP, NodeOutputBP, dtypes, input_widgets
+            >>> from ironflow.custom_nodes import Node, NodeInputBP, NodeOutputBP, dtypes, input_widgets
             >>> gui = GUI(script_title='foo')
             >>>
             >>> class MyNode(Node):
             >>>     title = "MyUserNode"
             >>>     init_inputs = [
             >>>         NodeInputBP(dtype=dtypes.Integer(default=1), label="foo")
             >>>     ]
@@ -251,43 +244,11 @@
         node_group: Optional[str] = None,
     ) -> None:
         if isinstance(source, (str, Path)):
             self.register_nodes_from_file(source, node_group=node_group)
         elif isinstance(source, types.ModuleType):
             self.register_nodes_from_module(source, node_group=node_group)
         elif isinstance(source, (list, tuple)) and all(
-            issubclass(item, Node) for item in source
+            [issubclass(item, Node) for item in source]
         ):
             for node_class in source:
                 self.register_node(node_class, node_group=node_group)
-
-    def recommend_nodes(self, port: NodeInput | NodeOutput):
-        recommendations = {}
-        if port.otype is not None:
-            if isinstance(port, NodeInput):
-                recommendations = self._get_nodes_giving_matching_output(port)
-            elif isinstance(port, NodeOutput):
-                recommendations = self._get_nodes_taking_matching_input(port)
-        self.nodes_dictionary["recommended"] = recommendations
-
-    def _get_nodes_giving_matching_output(self, port: NodeInput):
-        requirements = port.get_downstream_requirements()
-        sources = port.otype.get_sources(requirements)
-        return {
-            node.title: node
-            for node in self.session.nodes
-            if any(out.otype in sources for out in node.init_outputs)
-        }
-
-    def _get_nodes_taking_matching_input(self, port: NodeOutput):
-        return {
-            node.title: node
-            for node in self.session.nodes
-            if any(
-                port.otype in inp.otype.get_sources()
-                for inp in node.init_inputs
-                if inp.otype is not None
-            )
-        }
-
-    def clear_recommended_nodes(self):
-        self.nodes_dictionary["recommended"] = {}
```

### Comparing `ironflow-0.1.0/ironflow/model/node.py` & `ironflow-0.post0.dev1/ironflow/nodes/pyiron/atomistics_nodes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,671 +1,692 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
+"""
+Ryven nodes specifc to pyiron (or with ironflow improvements like an ipywidgets representation).
+"""
+
 from __future__ import annotations
 
-import inspect
+import json
 from abc import ABC, abstractmethod
-from typing import Callable, Optional
+from typing import TYPE_CHECKING
 
+import matplotlib.pylab as plt
 import numpy as np
-from owlready2 import Thing
+
 from pyiron_atomistics import Project
-from pyiron_base import GenericJob
-from ryvencore import Node as NodeCore
-from ryvencore.Base import Event
-from ryvencore.InfoMsgs import InfoMsgs
-from ryvencore.NodePort import NodePort
-from ryvencore.utils import deserialize
-
-from ironflow.gui.workflows.canvas_widgets.nodes import NodeWidget
-from ironflow.model import dtypes
-from ironflow.model.otypes import otype_from_str
-from ironflow.model.port import NodeInput, NodeInputBP, NodeOutput, NodeOutputBP
-from ironflow.utils import display_string
-
-
-class PortList(list):
-    """
-    When used to hold a collection of `NodePort` objects, the values of these ports then become accessible by their
-    labels, as long as those labels do not match an existing method of the builtin list class.
-
-    Warning:
-        This class makes no check that these labels are unique; if multiple items have the same label, the first one
-        is returned.
-
-    Warning:
-        Accessing port values in this way side-steps ryven functionality when in exec mode or using an executor
-        (i.e. when `running_with_executor`).
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(self, *args, **kwargs)
-        self._port_finder = PortFinder(self)
-        self._value_finder = ValueFinder(self)
-        # This additional mis-direction is necessary so that ports can have the same labels as list class methods
+from pyiron_atomistics.atomistics.structure.factory import StructureFactory
+from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
+from pyiron_atomistics.lammps import list_potentials
 
-    @property
-    def ports(self):
-        """
-        Allows attribute-like access to ports by their `label_str`
-        """
-        return self._port_finder
+from ironflow.gui.canvas_widgets import ButtonNodeWidget
+from ironflow.model import dtypes, NodeInputBP, NodeOutputBP
+from ironflow.model.node import Node
+from ironflow.nodes.std.special_nodes import DualNodeBase
 
-    @property
-    def values(self):
-        """
-        Allows attribute-like access to port values by their `label_str`
-
-        Calling `port_list.values.some_label` is equivalent to `port_list.ports.some_label.val`
-        """
-        return self._value_finder
+if TYPE_CHECKING:
+    from pyiron_base import HasGroups
 
-    @property
-    def labels(self):
-        return [item.label_str if isinstance(item, NodePort) else None for item in self]
+STRUCTURE_FACTORY = StructureFactory()
 
 
-class PortFinder:
-    def __init__(self, port_list: PortList):
-        self._port_list = port_list
+class BeautifulHasGroups:
+    """
+    A helper class for giving classes that inherit from `pyiron_base.HasGroups` a more appealing representation in
+    ipywidgets.
+    """
 
-    @property
-    def _filtered_port_list(self):
-        return [item for item in self._port_list if isinstance(item, NodePort)]
+    def __init__(self, has_groups: HasGroups | None):
+        self._has_groups = has_groups
 
-    def __getattr__(self, key):
-        for node_port in self._filtered_port_list:
-            if node_port.label_str == key:
-                return node_port
-        raise AttributeError(f"No port found with the label {key}")
+    def to_builtin(self, has_groups=None):
+        has_groups = has_groups if has_groups is not None else self._has_groups
+        if has_groups is not None:
+            repr_dict = {}
+            for k in has_groups.list_groups():
+                repr_dict[k] = self.to_builtin(has_groups[k])
+            for k in has_groups.list_nodes():
+                repr_dict[k] = str(has_groups[k])
+            return repr_dict
+        else:
+            return None
 
-    def __getitem__(self, item):
-        return self.__getattr__(item)
+    def _repr_json_(self):
+        return self.to_builtin()
 
-    def __iter__(self):
-        return self._filtered_port_list.__iter__()
+    def _repr_html_(self):
+        name = self._has_groups.__class__.__name__
+        plain = f"{name}({json.dumps(self.to_builtin(), indent=2, default=str)})"
+        return "<pre>" + plain + "</pre>"
 
-    def __len__(self):
-        return len(self._port_list)
 
+class Project_Node(Node):
+    """
+    Create a pyiron project.
 
-class ValueFinder(PortFinder):
-    def __getattr__(self, key):
-        node_port = super().__getattr__(key)
-        return node_port.val
+    Inputs:
+        name (str): The name of the project. Will access existing project data under that name. (Default is ".".)
 
-    def __iter__(self):
-        val_list = [p.val for p in self._filtered_port_list]
-        return val_list.__iter__()
+    Outputs:
+        project (pyiron_atomistics.Project): The project object.
+    """
 
+    # this __doc__ string will be displayed as tooltip in the editor
 
-class Node(NodeCore):
-    """
-    A parent class for all ironflow nodes. Apart from a small quality-of-life difference where outputs are
-    accessible in the same way as inputs (i.e. with a method `output(i)`), the main change here is the `before_update`
-    and `after_update` events. Callbacks to happen before and after the update can be added to (removed from) these with
-    the `connect` (`disconnect`) methods on the event. Such callbacks need to take the node itself as the first
-    argument, and the integer specifying which input channel is being updated as the second argument.
+    title = "Project"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Char(default="."), label="name"),
+    ]
+    init_outputs = [
+        NodeOutputBP(label="project"),
+    ]
+    color = "#aabb44"
 
-    Also provides a "representation" that gets used in the GUI to give a more detailed look at node data, which defaults
-    to showing output channel values.
+    def place_event(self):
+        super().place_event()
+        self.update()
 
-    Children should specify a title and some combination of initial input, output, and what to do when updated, e.g.:
+    def update_event(self, inp=-1):
+        pr = Project(self.input(0))
+        self.set_output_val(0, pr)
 
-    >>> class My_Node(Node):
-    >>>     title = "MyUserNode"
-    >>>     init_inputs = [
-    >>>         NodeInputBP(dtype=dtypes.Integer(default=1), label="foo")
-    >>>     ]
-    >>>     init_outputs = [
-    >>>        NodeOutputBP(label="bar")
-    >>>     ]
-    >>>     color = 'cyan'
-    >>>
-    >>> def update_event(self, inp=-1):
-    >>>     self.set_output_val(0, self.input(0) + 42)
+    @property
+    def _project(self):
+        return self.output(0)
 
-    Note:
-        When registering nodes from a module or .py file, only children of this class with names ending in `_Node` will
-        get registered.
-    """
+    @property
+    def representations(self) -> dict:
+        return {
+            "name": str(self.input(0)),
+            # "job_table": self._project.job_table() if self._project is not None else None
+            # Todo: Figure out how to display this without breaking the gui size; right now it automatically grows
+            # the gui because the table is so wide.
+        }
 
-    main_widget_class = NodeWidget
 
-    color = "#ff69b4"  # Add an abrasive default color -- won't crash if you forget to add one, but pops out a bit
+class OutputsOnlyAtoms(Node, ABC):
+    """
+    A helper class that manages representations for nodes whose only output is a `pyiron_atomistics.Atoms` object.
 
-    def __init__(self, params):
-        super().__init__(params)
-        self.inputs = PortList()
-        self.outputs = PortList()
+    Outputs:
+        structure (pyiron_atomistics.Atoms): An atomic structure.
+    """
 
-        self.before_update = Event(self, int)
-        self.after_update = Event(self, int)
-        self.actions = (
-            dict()
-        )  # Resolves Todo from ryven.NENV, moving it to our node class instead of ryvencore
-
-        self.representation_updated = False
-        self.after_update.connect(self._representation_update)
-
-    def _add_io(self, io_group, new_io, insert: int = None):
-        if insert is not None:
-            io_group.insert(insert, new_io)
-        else:
-            io_group.append(new_io)
+    init_outputs = [
+        NodeOutputBP(label="structure"),
+    ]
+    color = "#aabb44"
 
-    def create_input(
-        self,
-        type_: str = "data",
-        label: str = "",
-        add_data: Optional[dict] = None,
-        dtype: Optional[dtypes.DType] = None,
-        otype: Optional[Thing] = None,
-        insert: Optional[int] = None,
-    ):
-        """Creates and add a new input port"""
-        inp = NodeInput(
-            node=self,
-            type_=type_,
-            label_str=label,
-            add_data=add_data,
-            dtype=dtype,
-            otype=otype,
-        )
-        self._add_io(self.inputs, inp, insert=insert)
+    @abstractmethod
+    def update_event(self, inp=-1):
+        """Must set output 0 to an instance of pyiron_atomistics.atomistics.atoms.Atoms"""
+        pass
 
-    def create_input_dt(
-        self, dtype: dtypes.DType, label: str = "", add_data={}, insert: int = None
-    ):
-        raise RuntimeError(
-            "Ironflow uses custom NodePort classes and this method is not supported. "
-            "Please use create_input instead."
-        )
+    @property
+    def representations(self) -> dict:
+        return {"plot3d": self.output(0).plot3d(), "print": self.output(0)}
 
-    def create_output(
-        self,
-        type_: str = "data",
-        label: str = "",
-        dtype: Optional[dtypes.DType] = None,
-        otype: Optional[Thing] = None,
-        insert: Optional[int] = None,
-    ):
-        """Create and add a new output port"""
-        out = NodeOutput(
-            node=self,
-            type_=type_,
-            label_str=label,
-            dtype=dtype,
-            otype=otype,
-        )
-        self._add_io(self.outputs, out, insert=insert)
 
-    def _load_otype(self, data: dict):
-        try:
-            return otype_from_str(data["otype_namespace"], data["otype_name"])
-        except KeyError:
-            return None
+class BulkStructure_Node(OutputsOnlyAtoms):
+    """
+    Generate a bulk atomic structure.
 
-    def setup_ports(self, inputs_data=None, outputs_data=None):
-        # A streamlined version of the ryvencore method which exploits our NodeInput
-        # and NodeOutput classes instead, and for which all ports have a dtype
-        if not inputs_data and not outputs_data:
-            for i in range(len(self.init_inputs)):
-                inp = self.init_inputs[i]
-                self.create_input(
-                    type_=inp.type_,
-                    label=inp.label,
-                    add_data=inp.add_data,
-                    dtype=inp.dtype,
-                    otype=inp.otype,
-                )
-
-            for o in range(len(self.init_outputs)):
-                out = self.init_outputs[o]
-                self.create_output(
-                    type_=out.type_,
-                    label=out.label,
-                    dtype=out.dtype,
-                    otype=out.otype,
-                )
+    Inputs:
+        element (str): The atomic symbol for the desired atoms. (Default is "Fe".)
+        crystal_structure (str | None): Must be one of sc, fcc, bcc, hcp, diamond, zincblende,
+                                rocksalt, cesiumchloride, fluorite or wurtzite.
+        a (float | None): Lattice constant.
+        c (float | None): Lattice constant.
+        c_over_a (float | None): c/a ratio used for hcp.  Default is ideal ratio: sqrt(8/3).
+        u (float | None): Internal coordinate for Wurtzite structure.
+        orthorhombic (bool): Construct orthorhombic unit cell instead of primitive cell. (Takes precedence over cubic
+            flag when both are true.)
+        cubic (bool): Construct cubic unit cell if possible.
 
-        else:
-            # load from data
-            # initial ports specifications are irrelevant then
+    Outputs:
+        structure (pyiron_atomistics.Atoms): A mono-species bulk structure.
+    """
 
-            for inp in inputs_data:
-                dtype = dtypes.DType.from_str(inp["dtype"])(
-                    _load_state=deserialize(inp["dtype state"])
-                )
-                self.create_input(
-                    type_=inp["type"],
-                    label=inp["label"],
-                    add_data=inp,
-                    dtype=dtype,
-                    otype=self._load_otype(inp),
-                )
-
-                if "val" in inp:
-                    # this means the input is 'data' and did not have any connections,
-                    # so we saved its value which was probably represented by some
-                    # widget in the front end which has probably overridden the
-                    # Node.input() method
-                    self.inputs[-1].val = deserialize(inp["val"])
-                    self.inputs[-1].set_dtype_ok()
-
-            for out in outputs_data:
-                dtype = dtypes.DType.from_str(out["dtype"])(
-                    _load_state=deserialize(out["dtype state"])
-                )
-                self.create_output(
-                    type_=out["type"],
-                    label=out["label"],
-                    dtype=dtype,
-                    otype=self._load_otype(out),
-                )
+    # this __doc__ string will be displayed as tooltip in the editor
 
-    @property
-    def all_input_is_valid(self):
-        return all(p.ready for p in self.inputs.ports)
+    title = "BulkStructure"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Char(default="Fe"), label="element"),
+        NodeInputBP(
+            dtype=dtypes.Choice(
+                default=None,
+                items=[
+                    None,
+                    "sc",
+                    "fcc",
+                    "bcc",
+                    "hcp",
+                    "diamond",
+                    "zincblende",
+                    "rocksalt",
+                    "cesiumchloride",
+                    "fluorite",
+                    "wurtzite",
+                ],
+            ),
+            label="crystal_structure",
+        ),
+        NodeInputBP(dtype=dtypes.Float(default=None), label="a"),
+        NodeInputBP(dtype=dtypes.Float(default=None), label="c"),
+        NodeInputBP(dtype=dtypes.Float(default=None), label="c_over_a"),
+        NodeInputBP(dtype=dtypes.Float(default=None), label="u"),
+        NodeInputBP(dtype=dtypes.Boolean(default=False), label="orthorhombic"),
+        NodeInputBP(dtype=dtypes.Boolean(default=False), label="cubic"),
+    ]
+
+    def update_event(self, inp=-1):
+        self.set_output_val(
+            0,
+            STRUCTURE_FACTORY.bulk(
+                self.input(0),
+                crystalstructure=self.input(1),
+                a=self.input(2),
+                c=self.input(3),
+                covera=self.input(4),
+                u=self.input(5),
+                orthorhombic=self.input(6),
+                cubic=self.input(7),
+            ),
+        )
 
     def place_event(self):
-        # place_event() is executed *before* the connections are built
         super().place_event()
-        for inp in self.inputs:
-            if (
-                inp.val is None
-            ):  # Don't over-write data from loaded sessions with defaults
-                if inp.dtype is not None:
-                    inp.update(inp.dtype.default)
-                elif "val" in inp.add_data.keys():
-                    inp.update(inp.add_data["val"])
-
-    def update(self, inp=-1):
-        self.before_update.emit(self, inp)
-        super().update(inp=inp)
-        self.after_update.emit(self, inp)
-
-    def output(self, i):
-        return self.outputs[i].val
-
-    @staticmethod
-    def _representation_update(self, inp):
-        self.representation_updated = True
+        self.update()
 
-    @property
-    def _source_code(self):
-        try:
-            return inspect.getsource(self.__class__)
-        except TypeError:
-            # Classes defined in the notebook can't access their source this way
-            return ""
 
-    @property
-    def _standard_representations(self):
-        standard_reps = {
-            o.label_str if o.label_str != "" else f"output{i}": o.val
-            for i, o in enumerate(self.outputs)
-            if o.type_ == "data"
-        }
-        try:
-            standard_reps["source code"] = display_string(self._source_code)
-        except OSError:
-            # No source code can be found for user nodes defined in the nodebook
-            # But the source is available there anyhow
-            pass
-        return standard_reps
+class Repeat_Node(OutputsOnlyAtoms):
+    """
+    Repeat atomic structure supercell.
 
-    @property
-    def extra_representations(self):
-        """
-        When developing nodes, override this with any desired additional representations.
-
-        Note that standard representations exist for all output ports using the port's label (where available), so if
-        you add a key here matching one of those labels, you will override the standard output.
-        """
-        return {}
+    Inputs:
+        structure (pyiron_atomistics.Atoms): The structure to repeat periodically.
+        all (int): The number of times to repeat it in each of the three bravais lattice directions.
 
-    @property
-    def representations(self) -> dict:
-        return {**self._standard_representations, **self.extra_representations}
+    Outputs:
+        structure (pyiron_atomistics.Atoms): A repeated copy of the input structure.
+    """
 
-    def set_all_outputs_to_none(self):
-        for i in range(len(self.outputs)):
-            self.set_output_val(i, None)
+    # this __doc__ string will be displayed as tooltip in the editor
 
+    title = "Repeat"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="structure"),
+        NodeInputBP(dtype=dtypes.Integer(default=1, bounds=(1, 100)), label="all"),
+    ]
 
-class PlaceholderWidgetsContainer:
+    def update_event(self, inp=-1):
+        self.set_output_val(0, self.input(0).repeat(self.input(1)))
+
+
+class ApplyStrain_Node(OutputsOnlyAtoms):
     """
-    An object that just returns None for all accessed attributes so widgets.MyWidget in the non-ironflow nodes files
-    just returns None.
+    Apply strain on atomic structure supercell.
+
+    Inputs:
+        structure (pyiron_atomistics.Atoms): The atomic structure to strain.
+        strain (float): The isotropic strain to apply, where 0 is unstrained. (Default is 0.)
+
+    Outputs:
+        (pyiron_atomistics.Atoms): A strained copy of the input structure.
     """
 
-    def __getattr__(self, item):
-        return None
+    title = "ApplyStrain"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="structure"),
+        NodeInputBP(dtype=dtypes.Float(default=0, bounds=(-100, 100)), label="strain"),
+    ]
+
+    def update_event(self, inp=-1):
+        self.set_output_val(
+            0, self.input(0).apply_strain(float(self.input(1)), return_box=True)
+        )
 
 
-class BatchingNode(Node, ABC):
+class Lammps_Node(Node):
     """
-    A node whose update behaviour supports batched inputs.
+    WIP.
     """
 
-    @property
-    def batched_inputs(self):
-        return {
-            inp.label_str: inp
-            for inp in self.inputs
-            if inp.type_ == "data" and inp.dtype.batched
-        }
+    title = "Lammps"
+    version = "v0.1"
+    init_inputs = [
+        NodeInputBP(type_="exec", label="run"),
+        NodeInputBP(type_="exec", label="remove"),
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="project"),
+        NodeInputBP(dtype=dtypes.Char(default="job"), label="name"),
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="structure"),
+        NodeInputBP(
+            dtype=dtypes.Choice(
+                default="Set structure first", items=["Set structure first"]
+            ),
+            label="potential",
+        ),
+    ]
+    init_outputs = [
+        NodeOutputBP(type_="exec"),
+        NodeOutputBP(label="job"),
+    ]
+    color = "#5d95de"
 
     @property
-    def unbatched_inputs(self):
-        return {
-            inp.label_str: inp
-            for inp in self.inputs
-            if inp.type_ == "data" and not inp.dtype.batched
-        }
+    def _project(self):
+        return self.input(2)
 
     @property
-    def batched(self):
-        return len(self.batched_inputs) > 0
+    def _name(self):
+        return self.input(3)
 
     @property
-    def batch_lengths(self):
-        return {k: len(v.val) for k, v in self.batched_inputs.items()}
+    def _structure(self):
+        return self.input(4)
 
     @property
-    def _unbatched_kwargs(self):
-        return {k: v.val for k, v in self.unbatched_inputs.items()}
+    def _potential(self):
+        return self.input(5)
 
-    @property
-    def _batched_kwargs(self):
-        return [
-            {
-                k: v.val[i]
-                for k, v in zip(
-                    self.batched_inputs.keys(), self.batched_inputs.values()
-                )
-            }
-            for i in range(list(self.batch_lengths.values())[0])
-        ]
-
-    def generate_output(self) -> dict:
-        if self.batched:
-            batch_length_vals = list(self.batch_lengths.values())
-            if len(batch_length_vals) > 0 and not np.all(
-                np.array(batch_length_vals) == batch_length_vals[0]
-            ):
-                raise ValueError(
-                    f"Not all batch lengths are the same: {self.batch_lengths}"
-                )
-            return self.generate_batched_output()
+    def _run(self):
+        job = self._project.create.job.Lammps(self._name)
+        job.structure = self._structure
+        job.potential = self._potential
+        self._job = job
+        job.run()
+        self.set_output_val(1, job)
+        self.exec_output(0)
+
+    def _remove(self):
+        try:
+            name = (
+                self._job.name
+            )  # Remove based on the run job, not the input name which might have changed...
+            self._project.remove_job(name)
+            self.set_output_val(1, None)
+        except AttributeError:
+            pass
+
+    def _update_potential_choices(self):
+        potl_input = self.inputs[5]
+        last_potential = potl_input.val
+        structure = self.inputs[4].val
+        available_potentials = list_potentials(structure)
+
+        if len(available_potentials) == 0:
+            potl_input.val = "No valid potential"
+            potl_input.dtype.items = ["No valid potential"]
         else:
-            return self.generate_unbatched_output()
+            if last_potential not in available_potentials:
+                potl_input.val = available_potentials[0]
+            potl_input.dtype.items = available_potentials
 
-    def generate_unbatched_output(self):
-        return self.node_function(**self._unbatched_kwargs)
+    def update_event(self, inp=-1):
+        if inp == 0:
+            self._run()
+        elif inp == 1:
+            self._remove()
+        elif inp == 4:
+            self._update_potential_choices()
 
-    def generate_batched_output(self):
-        outputs = []
-        for i, kwargs in enumerate(self._batched_kwargs):
-            kwargs.update(self._unbatched_kwargs)
-            outputs.append(self.node_function(batch_index=i, **kwargs))
-        return {key: [d[key] for d in outputs] for key in outputs[0].keys()}
+    @property
+    def representations(self) -> dict:
+        return {"job": BeautifulHasGroups(self.output(1))}
 
-    def set_output(self):
-        try:
-            output = self.generate_output()
-        except Exception as e:
-            self.clear_output()
-            raise e
-        for k, v in output.items():
-            self.outputs.ports[k].dtype.batched = self.batched
-            self.outputs.ports[k].set_val(v)
-
-    def clear_output(self):
-        for p in self.outputs.ports:
-            if p.type_ == "data":
-                p.set_val(None)
-                p.dtype.batched = self.batched
-
-    def batched_representation(
-        self, label: str, representation_function: Callable, *args
-    ) -> dict | None:
-        """
-        Batched output requires multiple representations instead of a single one. Use
-        this function to wrap a function that produces your desired representation.
-        Resulting batched representations simply get an index added to their label.
-
-        Args:
-            label (str): The name of the representation.
-            representation_function (Callable): A function producing the representation.
-            *args: Members of `self.inputs.values` or `self.outputs.values` needed for
-                the representation.
-
-        Returns:
-            (dict): The representation(s).
-
-        Examples:
-            >>> def extra_representations(self):
-            >>>     return {
-            >>>         **self.batched_representation(
-            >>>             "bigger", self._add5, self.outputs.values.n
-            >>>        )
-            >>>     }
-            >>>
-            >>> @staticmethod
-            >>> def _add5(n: int):
-            >>>     return n + 5
-        """
-        try:
-            if self.batched:
-                return {
-                    f"{label}_{i}": representation_function(*batch_args)
-                    for i, batch_args in enumerate(zip(*args))
-                }
-            else:
-                return {label: representation_function(*args)}
-        except Exception as e:
-            return {label: f"Failed with: {e}"}
 
-    @abstractmethod
-    def node_function(self, *args, **kwargs) -> dict:
-        """
-        Takes all data input as kwargs, must return a dict with one entry for each data
-        output
-        """
-        pass
+class GenericOutput_Node(Node):
+    """
+    Select Generic Output item.
+
+    Inputs:
+        job (AtomisticGenericJob): A job with an `output` attribute of type
+            `pyiron_atomistics.atomistics.job.atomistic.GenericOutput`.
+        field (dtypes.Choice): Which output field to look at. Automatically populates once the job is valid.
+
+    Outputs:
+        output (numpy.ndarray): The selected output field.
+    """
+
+    version = "v0.1"
+    title = "GenericOutput"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="job"),
+        NodeInputBP(
+            dtype=dtypes.Choice(
+                default="Input an atomistic job", items=["Input an atomistic job"]
+            ),
+            label="field",
+        ),
+    ]
+    init_outputs = [
+        NodeOutputBP(label="output"),
+    ]
+    color = "#c69a15"
+
+    def __init__(self, params):
+        super().__init__(params)
+
+    @property
+    def _job(self):
+        return self.input(0)
 
+    def _update_fields(self):
+        if isinstance(self._job, AtomisticGenericJob):
+            self.inputs[1].dtype.items = self._job["output/generic"].list_nodes()
+            self.inputs[1].val = self.inputs[1].dtype.items[0]
+        else:
+            self.inputs[1].dtype.items = [self.init_inputs[1].dtype.default]
+            # Note: It would be sensible to use `self.init_outputs[1].dtype.items` above, but this field gets updated
+            # to `self.inputs[1].dtype.items`, probably because of the mutability of lists.
+            self.inputs[1].val = self.init_inputs[1].dtype.default
+
+    def _update_value(self):
+        if isinstance(self._job, AtomisticGenericJob):
+            val = self._job[f"output/generic/{self.input(1)}"]
+        else:
+            val = None
+        self.set_output_val(0, val)
+
+    def update_event(self, inp=-1):
+        if inp == 0:
+            self._update_fields()
+            self._update_value()
+        elif inp == 1:
+            self._update_value()
 
-class DataNode(BatchingNode, ABC):
+
+class IntRand_Node(Node):
     """
-    A node that can update as soon as all input is valid and produces output data.
+    Generate a random non-negative integer.
+
+    Inputs:
+        high (int): Biggest possible integer. (Default is 1).
+        length (int): How many random numbers to generate. (Default is 1.)
+
+    Outputs:
+        randint (int|numpy.ndarray): The randomly generated value(s).
     """
 
+    # this __doc__ string will be displayed as tooltip in the editor
+
+    title = "IntRandom"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Integer(default=1, bounds=(10, 100)), label="high"),
+        NodeInputBP(dtype=dtypes.Integer(default=1, bounds=(1, 100)), label="length"),
+    ]
+    init_outputs = [
+        NodeOutputBP(label="randint"),
+    ]
+    color = "#aabb44"
+
     def update_event(self, inp=-1):
-        if self.all_input_is_valid:
-            self.set_output()
-        else:
-            self.clear_output()
+        val = np.random.randint(0, high=self.input(0), size=self.input(1))
+        self.set_output_val(0, val)
 
-    def place_event(self):
-        super().place_event()
-        self.update()
 
+class JobName_Node(Node):
+    """
+    Create job name for parameters.
+
+    Inputs:
+        base (str): The stem for the final name. (Default is "job_".)
+        float (float): The parameter value to add to the name.
+
+    Outputs:
+        job_name (str): The base plus float sanitized into a valid job name.
 
-class JobNode(BatchingNode, ABC):
+    Todo:
+        There has been some work in pyiron_base on getting a cleaner job name sanitizer, so lean on that.
     """
-    A parent class for nodes that run a pyiron job.
 
-    Child classes are required to specify a `_generate_job` method, which takes the
-    node input data and returns a `pyiron_base.GenericJob` object, and (optionally) a
-    `_get_output_from_job` method which takes the executed job and the node input data
-    and returns a dictionary of output with keys corresponding to node output port
-    labels. The `job` output type can be made more specific with the `valid_job_classes`
-    class attribute.
+    title = "JobName"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Char(default="job_"), label="base"),
+        NodeInputBP(dtype=dtypes.Float(default=0), label="float"),
+    ]
+    init_outputs = [
+        NodeOutputBP(label="job_name"),
+    ]
+    color = "#aabb44"
 
-    In the event that some of the input is batched but the `name` input is *not*
-    batched, then the `name` argument passed to `_generate_job` is automatically
-    appended with batch index information to prevent jobs from having the same name.
+    def update_event(self, inp=-1):
+        val = self.input(0) + f"{float(self.input(1))}".replace("-", "m").replace(
+            ".", "p"
+        )
+        self.set_output_val(0, val)
 
-    The node has `run` and `remove` input exec ports and a `ran` output exec port.
-    Once the node has been run, all inputs get locked and remain locked until the
-    removal process is triggered. Remove clears all the outputs and sets them to `None`.
 
-    If a failure is encountered during the `run` process, the exception is raised, all
-    pyiron jobs are deleted (this might need to change if we want to do more expensive
-    jobs in the future!), the node output is cleared, and the offending exception is
-    raised to the log.
+class Linspace_Node(Node):
+    """
+    Generate a linear mesh in a given range using `np.linspace`.
 
-    All descendant classes from this node class expect to have `run`, `remove`, and
-    `name` input, and `ran` output. Therefore, when defining additional ports, use this
-    format:
+    Inputs:
+        min (int): The lower bound (inclusive). (Default is 1.)
+        max (int): The upper bound (inclusive). (Default is 2.)
+        steps (int): How many samples to take inside (min, max). (Default is 10.)
 
-    >>> init_inputs = JobNode.init_inputs + [WHATEVER_ELSE_YOU_WANT]
-    >>> init_outputs = JobNode.init_outputs + [OTHER_STUFF]
+    Outputs:
+        linspace (numpy.ndarray): A uniform sampling over the requested range.
     """
 
-    color = "#c4473f"
-    valid_job_classes = None
+    # this __doc__ string will be displayed as tooltip in the editor
+
+    title = "Linspace"
     init_inputs = [
-        NodeInputBP(type_="exec", label="run"),
-        NodeInputBP(type_="exec", label="reset"),
-        NodeInputBP(dtype=dtypes.String(default="calc"), label="name"),
+        NodeInputBP(dtype=dtypes.Integer(default=1, bounds=(0, 100)), label="min"),
+        NodeInputBP(dtype=dtypes.Integer(default=2, bounds=(0, 100)), label="max"),
+        NodeInputBP(dtype=dtypes.Integer(default=10, bounds=(1, 100)), label="steps"),
     ]
     init_outputs = [
-        NodeOutputBP(type_="exec", label="ran"),
-        NodeOutputBP(dtype=dtypes.Data(valid_classes=GenericJob), label="job"),
+        NodeOutputBP(label="linspace"),
     ]
+    color = "#aabb44"
 
     def place_event(self):
         super().place_event()
-        if self.valid_job_classes is not None:
-            self.outputs.ports.job.dtype.valid_classes = self.valid_job_classes
+        self.update()
 
     def update_event(self, inp=-1):
-        if inp == 0 and (not self.block_updates) and self.all_input_is_valid:
-            self.block_updates = True
-            try:
-                self._jobs = []
-                self.set_output()
-                self.exec_output(0)
-            except Exception as e:
-                self._on_remove_signal()
-                raise e
-        else:
-            self.clear_output()
+        val = np.linspace(self.input(0), self.input(1), self.input(2))
+        self.set_output_val(0, val)
 
-    def update(self, inp=-1):
-        if inp == 1:
-            # Bypass the `lock_updates` to delete the executed job and unlock updates
-            self._on_remove_signal()
-            # self.update(-1)
-        else:
-            super().update(inp=inp)
 
-    def node_function(self, name, *args, **kwargs):
-        if self.batched and not self.inputs.ports.name.dtype.batched:
-            name = f"{name}_batch{kwargs['batch_index']}"
-        job = self._raise_error_if_not_initialized(
-            self._generate_job(name, *args, **kwargs)
-        )
-        self._jobs.append(job)
-        job.run()
-        data = self._get_output_from_job(job, *args, name=name, **kwargs)
-        return {
-            "job": job,
-            **data,
-        }
+class Plot3d_Node(Node):
+    """
+    Plot a structure with NGLView.
 
-    def _on_remove_signal(self):
-        if hasattr(self, "_jobs"):
-            for job in self._jobs:
-                job.remove()
-        self.clear_output()
-        self.block_updates = False
-
-    def _raise_error_if_not_initialized(self, job: GenericJob) -> GenericJob:
-        if job.status == "initialized":
-            return job
-        else:
-            self.block_updates = False
-            raise RuntimeError(
-                f"The job {self.inputs.values.name} already exists. Delete it first or"
-                f"choose a different name."
-            )
+    Inputs:
+        structure (pyiron_atomistics.Atoms): The structure to plot.
 
-    @abstractmethod
-    def _generate_job(self, name: str, *args, **kwargs) -> GenericJob:
-        """
-        Takes a (potentially modified[^1]) name and the rest of the input data and
-        returns a job to `.run()`
-
-        [^1]: If some of the input is batched, but the `name` field is not batched, the
-              batch index information will get automatically appended to the name.
-        """
-
-        pass
+    Outputs:
+        plot3d (nglview.widget.NGLWidget): The plot object.
+        structure (pyiron_atomistics.Atoms): The raw structure object passed in.
+    """
 
-    def _get_output_from_job(self, finished_job: GenericJob, *args, **kwargs) -> dict:
-        """
-        Takes the executed job and all the node input data, and should return relevant
-        output data as a dictionary with keys matching the output port labels.
-        """
+    title = "Plot3d"
+    version = "v0.1"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="structure"),
+    ]
+    init_outputs = [
+        NodeOutputBP(type_="data", label="plot3d"),
+        NodeOutputBP(type_="data", label="structure"),
+    ]
+    color = "#5d95de"
 
-        return {}
+    def update_event(self, inp=-1):
+        self.set_output_val(0, self.input(0).plot3d())
+        self.set_output_val(1, self.input(0))
 
 
-class JobMaker(JobNode, ABC):
+class Matplot_Node(Node):
     """
-    A job-running node that takes creates a new job instance from scratch, ready to
-    `.run()`.
+    A 2D matplotlib plot.
 
-    All descendant classes from this node class expect to have `run`, `remove`, `name`,
-    and `project` input, and `ran` output. Therefore, when defining additional ports,
-    use this format:
+    Inputs:
+        x (list|numpy.ndarray|...): Data for the x-axis.
+        y (list|numpy.ndarray|...): Data for the y-axis.
 
-    >>> init_inputs = JobMaker.init_inputs + [WHATEVER_ELSE_YOU_WANT]
-    >>> init_outputs = JobMaker.init_outputs + [OTHER_STUFF]
+    Outputs:
+        fig (matplotlib.figure.Figure): The resulting figure after a `matplotlib.pyplot.plot` call on x and y.
     """
 
-    init_inputs = JobNode.init_inputs + [
-        NodeInputBP(dtype=dtypes.Data(valid_classes=Project), label="project")
+    title = "MatPlot"
+    version = "v0.1"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="x"),
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="y"),
     ]
+    init_outputs = [
+        NodeOutputBP(type_="data", label="fig"),
+    ]
+    color = "#5d95de"
 
+    def update_event(self, inp=-1):
+        super().update_event()
+        plt.ioff()
+        fig = plt.figure()
+        plt.clf()
+        plt.plot(self.input(0), self.input(1))
+        self.set_output_val(0, fig)
+        plt.ion()
 
-class JobTaker(JobNode, ABC):
-    """
-    A job-running node that takes a template job instance as input, and copies and
-    modifies it prior to use.
 
-    Valid classes for the `job` input can be overriden with the `valid_job_classes`
-    attribute.
+class Sin_Node(Node):
+    """
+    Call `numpy.sin` on a value.
 
-    All descendant classes from this node class expect to have `run`, `remove`, `name`,
-    and `job` input, and `ran` output. Therefore, when defining additional ports, use
-    this format:
+    Inputs:
+        x (int|float|list|numpy.ndarray|...): The value to sine transform.
 
-    >>> init_inputs = JobTaker.init_inputs + [WHATEVER_ELSE_YOU_WANT]
-    >>> init_outputs = JobTaker.init_outputs + [OTHER_STUFF]
+    Outputs:
+        sin (float|numpy.ndarray): The sine of x.
     """
 
-    init_inputs = JobNode.init_inputs + [
-        NodeInputBP(dtype=dtypes.Data(valid_classes=GenericJob), label="job")
+    title = "Sin"
+    version = "v0.1"
+    init_inputs = [
+        NodeInputBP(dtype=dtypes.Data(size="m"), label="x"),
+    ]
+    init_outputs = [
+        NodeOutputBP(label="sin"),
     ]
+    color = "#5d95de"
+
+    def update_event(self, inp=-1):
+        self.set_output_val(0, np.sin(self.input(0)))
+
+
+class Result_Node(Node):
+    """Simply shows a value converted to str"""
+
+    version = "v0.1"
+
+    title = "Result"
+    init_inputs = [
+        NodeInputBP(type_="data"),
+    ]
+    color = "#c69a15"
+
+    def __init__(self, params):
+        super().__init__(params)
+        self.val = None
 
     def place_event(self):
         super().place_event()
-        if self.valid_job_classes is not None:
-            self.inputs.ports.job.dtype.valid_classes = self.valid_job_classes
+        self.update()
 
-    def _generate_job(self, name: str, job: GenericJob, **kwargs) -> GenericJob:
-        copied_job = job.copy_to(new_job_name=name)
-        return self._modify_job(copied_job, **kwargs)
+    def view_place_event(self):
+        self.main_widget().show_val(self.val)
 
-    @abstractmethod
-    def _modify_job(self, copied_job: GenericJob, *args, **kwargs) -> GenericJob:
-        """
-        Takes the generated job, modifies it in place using the input data (except for
-        the `job` and `name` input values) and returns it ready to be `.run()`
-        """
-        pass
+    def update_event(self, inp=-1):
+        self.val = self.input(0)
+        if self.session.gui:
+            self.main_widget().show_val(self.val)
+
+
+class ForEach_Node(Node):
+    title = "ForEach"
+    version = "v0.1"
+    init_inputs = [
+        NodeInputBP(type_="exec", label="start"),
+        NodeInputBP(type_="exec", label="reset"),
+        NodeInputBP(dtype=dtypes.List(), label="elements"),
+    ]
+    init_outputs = [
+        NodeOutputBP(label="loop", type_="exec"),
+        NodeOutputBP(label="e", type_="data"),
+        NodeOutputBP(label="finished", type_="exec"),
+    ]
+    color = "#b33a27"
+
+    _count = 0
+
+    def update_event(self, inp=-1):
+        if inp == 0:
+            self._count += 1
+            if len(self.input(2)) > self._count:
+                e = self.input(2)[self._count]
+                self.set_output_val(1, e)
+                self.exec_output(0)
+            else:
+                self.exec_output(2)
+        elif inp > 0:
+            self._count = 0
+        self.val = self._count
+
+
+class ExecCounter_Node(DualNodeBase):
+    title = "ExecCounter"
+    version = "v0.1"
+    init_inputs = [
+        NodeInputBP(type_="exec"),
+    ]
+    init_outputs = [
+        NodeOutputBP(type_="exec"),
+    ]
+    color = "#5d95de"
+
+    def __init__(self, params):
+        super().__init__(params, active=True)
+        self._count = 0
+
+    def update_event(self, inp=-1):
+        if self.active and inp == 0:
+            self._count += 1
+            self.val = self._count
+        elif not self.active:
+            self.val = self.input(0)
+
+
+class Click_Node(Node):
+    title = "Click"
+    version = "v0.1"
+    main_widget_class = ButtonNodeWidget
+    init_inputs = []
+    init_outputs = [NodeOutputBP(type_="exec")]
+    color = "#99dd55"
+
+    def update_event(self, inp=-1):
+        self.exec_output(0)
+
+
+nodes = [
+    Project_Node,
+    BulkStructure_Node,
+    Repeat_Node,
+    ApplyStrain_Node,
+    Lammps_Node,
+    JobName_Node,
+    GenericOutput_Node,
+    Plot3d_Node,
+    IntRand_Node,
+    Linspace_Node,
+    Sin_Node,
+    Result_Node,
+    ExecCounter_Node,
+    Matplot_Node,
+    Click_Node,
+    ForEach_Node,
+]
```

### Comparing `ironflow-0.1.0/ironflow/node_tools/__init__.py` & `ironflow-0.post0.dev1/ironflow/custom_nodes/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
-The necessary classes for creating new nodes.
+The necessary classes for creating custom nodes.
 
 Example:
     >>> from ironflow import GUI
-    >>> from ironflow.node_tools import Node, NodeInputBP, NodeOutputBP, dtypes, input_widgets
+    >>> from ironflow.custom_nodes import Node, NodeInputBP, NodeOutputBP, dtypes, input_widgets
     >>> gui = GUI(script_title='foo')
     >>>
     >>> class MyNode(Node):
     >>>     title = "MyUserNode"
     >>>     init_inputs = [
     >>>         NodeInputBP(dtype=dtypes.Integer(default=1), label="foo")
     >>>     ]
@@ -21,21 +21,10 @@
     >>>
     >>>     def update_event(self, inp=-1):
     >>>         self.set_output_val(0, self.input(0) + 42)
     >>>
     >>> gui.register_node(MyNode)
 """
 
-import ironflow.node_tools.input_widgets
-import ironflow.node_tools.main_widgets
-from ironflow.model import dtypes
-from ironflow.model.node import (
-    Node,
-    PlaceholderWidgetsContainer,
-    PortList,
-    BatchingNode,
-    DataNode,
-    JobMaker,
-    JobNode,
-    JobTaker,
-)
-from ironflow.model.port import NodeInputBP, NodeOutputBP
+import ironflow.custom_nodes.input_widgets
+from ironflow.model import dtypes, NodeInputBP, NodeOutputBP
+from ironflow.model.node import Node
```

### Comparing `ironflow-0.1.0/ironflow/nodes/deprecated/basic_operators.py` & `ironflow-0.post0.dev1/ironflow/nodes/std/basic_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from ironflow.node_tools import dtypes, Node, NodeInputBP, NodeOutputBP
+from ironflow.model import dtypes, NodeInputBP, NodeOutputBP
+from ironflow.model.node import Node
 
 
 class OperatorNodeBase(Node):
+
     version = "v0.0"
 
     init_inputs = [
         NodeInputBP(dtype=dtypes.Data(size="s")),
         NodeInputBP(dtype=dtypes.Data(size="s")),
     ]
 
@@ -41,14 +43,15 @@
         self.actions[f"remove input {index}"] = {
             "method": self.remove_operand_input,
             "data": index,
         }
         self.num_inputs += 1
 
     def rebuild_remove_actions(self):
+
         remove_keys = []
         for k, v in self.actions.items():
             if k.startswith("remove input"):
                 remove_keys.append(k)
 
         for k in remove_keys:
             del self.actions[k]
```

### Comparing `ironflow-0.1.0/ironflow/nodes/deprecated/built_in.py` & `ironflow-0.post0.dev1/ironflow/nodes/built_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-from ironflow.node_tools import (
-    dtypes,
-    Node,
-    NodeInputBP,
-    NodeOutputBP,
-    PlaceholderWidgetsContainer,
-)
+from ironflow.model import dtypes, NodeInputBP, NodeOutputBP
+from ironflow.model.node import Node, PlaceholderWidgetsContainer
 
 widgets = PlaceholderWidgetsContainer()
 
 
 class NodeBase(Node):
     pass
 
@@ -16,15 +11,15 @@
 class GetVar_Node(NodeBase):
     """Gets the value of a script variable"""
 
     version = "v0.1"
 
     title = "get var"
     init_inputs = [
-        NodeInputBP(dtype=dtypes.String()),
+        NodeInputBP(dtype=dtypes.String(size="m")),
     ]
     init_outputs = [NodeOutputBP(label="val")]
     color = "#c69a15"
 
     def __init__(self, params):
         super().__init__(params)
 
@@ -35,14 +30,15 @@
         self.update()
 
     def view_place_event(self):
         self.var_name = self.input(0)
 
     def update_event(self, input_called=-1):
         if self.input(0) != self.var_name:
+
             if self.var_name != "":  # disconnect old var val update connection
                 self.unregister_var_receiver(self.var_name, self.var_val_changed)
 
             self.var_name = self.input(0)
 
             # create new var update connection
             self.register_var_receiver(self.var_name, self.var_val_changed)
@@ -88,15 +84,15 @@
     version = "v0.1"
 
     title = "val"
     init_inputs = [
         NodeInputBP(dtype=dtypes.Data(size="s")),
     ]
     init_outputs = [
-        NodeOutputBP(type_="data"),
+        NodeInputBP(type_="data"),
     ]
     style = "small"
     color = "#c69a15"
 
     def __init__(self, params):
         super().__init__(params)
 
@@ -128,14 +124,15 @@
     def get_state(self):
         return {"val": self.val}  # self.main_widget().get_val()
 
     def set_state(self, data, version):
         self.val = data["val"]
 
         if version is None:
+
             self.display_title = ""
 
             self.create_input_dt(dtype=dtypes.Data(size="s"))
 
             # the old version didn't use a dtype
             self.inputs[0].dtype.val = self.val
             self.inputs[0].update(self.val)
@@ -165,20 +162,23 @@
         self.actions["make passive"] = {"method": self.action_make_passive}
         self.active = True
 
         self.var_name = ""
         self.num_vars = 1
 
     def update_event(self, input_called=-1):
+
         if self.active and input_called == 0:
+
             if self.set_var_val(self.input(1), self.input(2)):
                 self.set_output_val(1, self.input(2))
             self.exec_output(0)
 
         elif not self.active:
+
             self.var_name = self.input(0)
             if self.set_var_val(self.input(0), self.input(1)):
                 self.set_output_val(0, self.get_var_val(self.var_name))
 
     def action_make_passive(self):
         self.active = False
         self.delete_input(0)
@@ -235,14 +235,15 @@
     def remove_var_input(self, number):
         self.delete_input((number - 1) * 2)
         self.delete_input((number - 1) * 2)
         self.num_vars -= 1
         self.rebuild_remove_actions()
 
     def rebuild_remove_actions(self):
+
         remove_keys = []
         for k, v in self.actions.items():
             if k.startswith("remove var"):
                 remove_keys.append(k)
 
         for k in remove_keys:
             del self.actions[k]
@@ -250,14 +251,15 @@
         for i in range(self.num_vars):
             self.actions[f"remove var {i+1}"] = {
                 "method": self.remove_var_input,
                 "data": i + 1,
             }
 
     def update_event(self, input_called=-1):
+
         var_names = [self.input(i) for i in range(0, len(self.inputs), 2)]
         values = [self.input(i) for i in range(1, len(self.inputs), 2)]
 
         for i in range(len(var_names)):
             self.set_var_val(var_names[i], values[i])
 
     def get_state(self):
```

### Comparing `ironflow-0.1.0/ironflow/nodes/deprecated/control_structures.py` & `ironflow-0.post0.dev1/ironflow/nodes/std/control_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ironflow.node_tools import dtypes, Node, NodeInputBP, NodeOutputBP
+from ironflow.model import dtypes, NodeInputBP, NodeOutputBP
+from ironflow.model.node import Node
 
 
 class CSNodeBase(Node):
     version = "v0.1"
     style = "normal"
     color = "#b33a27"
 
@@ -74,14 +75,15 @@
         self.delete_output(out_index)
         self.delete_output(out_index)
         self.dims -= 1
         # del self.actions[f'remove dimension {dim}']
         self.rebuild_remove_actions()
 
     def rebuild_remove_actions(self):
+
         remove_keys = []
         for k, v in self.actions.items():
             if k.startswith("remove dimension"):
                 remove_keys.append(k)
 
         for k in remove_keys:
             del self.actions[k]
@@ -100,20 +102,22 @@
 
     def update_event(self, inp=-1):
         if inp == 0:
             self.iterate(1)
             self.exec_output(len(self.outputs) - 1)
 
     def iterate(self, dim):
+
         inp_index = self.input_from_dim(dim)
 
         exec_out_index = self.output_from_dim(dim)
         data_out_index = exec_out_index + 1
 
         for i in range(self.input(inp_index), self.input(inp_index + 1)):
+
             self.set_output_val(data_out_index, i)
             self.exec_output(exec_out_index)
 
             if dim < self.dims:
                 self.iterate(dim + 1)
```

### Comparing `ironflow-0.1.0/ironflow/nodes/deprecated/special_nodes.py` & `ironflow-0.post0.dev1/ironflow/nodes/std/special_nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import code
 from contextlib import redirect_stdout, redirect_stderr
 
-from ironflow.node_tools import (
-    dtypes,
-    input_widgets,
-    Node,
-    NodeInputBP,
-    NodeOutputBP,
-    PlaceholderWidgetsContainer,
-)
+from ironflow.model import dtypes, NodeInputBP, NodeOutputBP
+from ironflow.model.node import Node, PlaceholderWidgetsContainer
+from ironflow.gui.boxes.node_interface.input_widgets import SliderControl
 
 widgets = PlaceholderWidgetsContainer()
 
 
 class NodeBase(Node):
     version = "v0.1"
     color = "#FFCA00"
@@ -277,14 +272,15 @@
     def __init__(self, params):
         super().__init__(params)
 
         self.actions["start"] = {"method": self.start}
         self.actions["stop"] = {"method": self.stop}
 
         if self.session.gui:
+
             from qtpy.QtCore import QTimer
 
             self.timer = QTimer(self)
             self.timer.timeout.connect(self.timeouted)
             self.iteration = 0
 
     def timeouted(self):
@@ -333,29 +329,30 @@
         NodeInputBP(dtype=dtypes.Boolean(default=False), label="round"),
     ]
     init_outputs = [
         NodeOutputBP(),
     ]
     main_widget_class = widgets.SliderNode_MainWidget
     main_widget_pos = "below ports"
-    input_widget = input_widgets.SliderControl
+    input_widget = SliderControl
 
     def __init__(self, params):
         super().__init__(params)
 
         self.val = 0
 
     def place_event(self):
         self.update()
 
     def view_place_event(self):
         # when running in gui mode, the value might come from the input widget
         self.update()
 
     def update_event(self, inp=-1):
+
         v = self.input(0) * self.val
         if self.input(1):
             v = round(v)
 
         self.set_output_val(0, v)
 
     def get_state(self) -> dict:
```

### Comparing `ironflow-0.1.0/ironflow.egg-info/SOURCES.txt` & `ironflow-0.post0.dev1/ironflow.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,62 +2,46 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 ironflow/__init__.py
 ironflow/_version.py
-ironflow/utils.py
 ironflow.egg-info/PKG-INFO
 ironflow.egg-info/SOURCES.txt
 ironflow.egg-info/dependency_links.txt
 ironflow.egg-info/requires.txt
 ironflow.egg-info/top_level.txt
+ironflow/custom_nodes/__init__.py
+ironflow/custom_nodes/input_widgets/__init__.py
 ironflow/gui/__init__.py
-ironflow/gui/base.py
-ironflow/gui/browser.py
-ironflow/gui/draws_widgets.py
 ironflow/gui/gui.py
-ironflow/gui/log.py
-ironflow/gui/workflows/__init__.py
-ironflow/gui/workflows/screen.py
-ironflow/gui/workflows/boxes/__init__.py
-ironflow/gui/workflows/boxes/base.py
-ironflow/gui/workflows/boxes/flow.py
-ironflow/gui/workflows/boxes/text_output.py
-ironflow/gui/workflows/boxes/toolbar.py
-ironflow/gui/workflows/boxes/user_input.py
-ironflow/gui/workflows/boxes/node_interface/__init__.py
-ironflow/gui/workflows/boxes/node_interface/control.py
-ironflow/gui/workflows/boxes/node_interface/input_widgets.py
-ironflow/gui/workflows/boxes/node_interface/representation.py
-ironflow/gui/workflows/canvas_widgets/__init__.py
-ironflow/gui/workflows/canvas_widgets/base.py
-ironflow/gui/workflows/canvas_widgets/buttons.py
-ironflow/gui/workflows/canvas_widgets/flow.py
-ironflow/gui/workflows/canvas_widgets/layouts.py
-ironflow/gui/workflows/canvas_widgets/nodes.py
-ironflow/gui/workflows/canvas_widgets/ports.py
+ironflow/gui/boxes/__init__.py
+ironflow/gui/boxes/base.py
+ironflow/gui/boxes/flow.py
+ironflow/gui/boxes/text_output.py
+ironflow/gui/boxes/toolbar.py
+ironflow/gui/boxes/user_input.py
+ironflow/gui/boxes/node_interface/__init__.py
+ironflow/gui/boxes/node_interface/base.py
+ironflow/gui/boxes/node_interface/control.py
+ironflow/gui/boxes/node_interface/input_widgets.py
+ironflow/gui/boxes/node_interface/representation.py
+ironflow/gui/canvas_widgets/__init__.py
+ironflow/gui/canvas_widgets/base.py
+ironflow/gui/canvas_widgets/buttons.py
+ironflow/gui/canvas_widgets/flow.py
+ironflow/gui/canvas_widgets/layouts.py
+ironflow/gui/canvas_widgets/nodes.py
+ironflow/gui/canvas_widgets/ports.py
 ironflow/model/__init__.py
 ironflow/model/dtypes.py
-ironflow/model/flow.py
 ironflow/model/model.py
 ironflow/model/node.py
-ironflow/model/otypes.py
-ironflow/model/port.py
-ironflow/model/script.py
-ironflow/model/session.py
-ironflow/node_tools/__init__.py
-ironflow/node_tools/main_widgets.py
-ironflow/node_tools/input_widgets/__init__.py
 ironflow/nodes/__init__.py
-ironflow/nodes/array.py
-ironflow/nodes/plot.py
-ironflow/nodes/pyiron_atomistics.py
-ironflow/nodes/standard.py
-ironflow/nodes/deprecated/__init__.py
-ironflow/nodes/deprecated/basic_operators.py
-ironflow/nodes/deprecated/built_in.py
-ironflow/nodes/deprecated/control_structures.py
-ironflow/nodes/deprecated/flow_control.py
-ironflow/nodes/deprecated/special_nodes.py
-tests/test_tests.py
+ironflow/nodes/built_in.py
+ironflow/nodes/pyiron/__init__.py
+ironflow/nodes/pyiron/atomistics_nodes.py
+ironflow/nodes/std/__init__.py
+ironflow/nodes/std/basic_operators.py
+ironflow/nodes/std/control_structures.py
+ironflow/nodes/std/special_nodes.py
```

### Comparing `ironflow-0.1.0/setup.py` & `ironflow-0.post0.dev1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,51 +3,40 @@
 """
 from setuptools import setup, find_packages
 import versioneer
 
 setup(
     name='ironflow',
     version=versioneer.get_version(),
-    description='ironflow - A visual scripting interface for pyiron.',
-    long_description='Ironflow combines ryven, ipycanvas and ipywidgets to provide a Jupyter-based visual scripting '
-                     'gui for running pyiron workflow graphs.',
+    description='ironflow - module extension to pyiron.',
+    long_description='http://pyiron.org',
 
     url='https://github.com/pyiron/ironflow',
     author='Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department',
     author_email='liamhuber@greyhavensolutions.com',
     license='BSD',
 
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Topic :: Scientific/Engineering :: Physics',
-        'License :: OSI Approved :: BSD License',
-        'Intended Audience :: Science/Research',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
+    classifiers=['Development Status :: 5 - Production/Stable',
+                 'Topic :: Scientific/Engineering :: Physics',
+                 'License :: OSI Approved :: BSD License',
+                 'Intended Audience :: Science/Research',
+                 'Operating System :: OS Independent',
+                 'Programming Language :: Python :: 3.7',
+                 'Programming Language :: Python :: 3.8',
+                 'Programming Language :: Python :: 3.9'],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
-        'aimsgb >=0.1.3',
-        'ipycanvas >=0.13.2',
-        'ipython >=8.24.0',
-        'ipywidgets >=7.7.1',
-        'jupyterlab >=3.6.7',
-        'matplotlib >=3.8.4',
-        'nglview >=3.0.8',
-        'numpy >=1.26.4',
-        'owlready2 >=0.46',
-        'pandas >=1.5.3',
-        'pyiron_atomistics >= 0.2.63',
-        'pyiron_base >=0.5.33',
-        'pyiron_gui <=0.0.8',
-        'pyiron_ontology >=0.1.3',
-        'pymatgen >=2023.5.10',
-        'ryvencore >=0.3.1.1',
-        'seaborn >=0.13.2',
-        'traitlets >=5.14.3',
+        'ipycanvas',
+        'ipython',
+        'ipywidgets >= 7,< 8',
+        'matplotlib',
+        'nglview',
+        'numpy',
+        'pyiron_base',
+        'pyiron_atomistics',
+        'ryvencore'
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `ironflow-0.1.0/versioneer.py` & `ironflow-0.post0.dev1/versioneer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,39 @@
 
-# Version: 0.29
+# Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/python-versioneer/python-versioneer
+* https://github.com/warner/python-versioneer
 * Brian Warner
-* License: Public Domain (Unlicense)
-* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
-* [![Latest Version][pypi-image]][pypi-url]
-* [![Build Status][travis-image]][travis-url]
+* License: Public Domain
+* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
+* [![Latest Version]
+(https://pypip.in/version/versioneer/badge.svg?style=flat)
+](https://pypi.python.org/pypi/versioneer/)
+* [![Build Status]
+(https://travis-ci.org/warner/python-versioneer.png?branch=master)
+](https://travis-ci.org/warner/python-versioneer)
 
-This is a tool for managing a recorded version number in setuptools-based
+This is a tool for managing a recorded version number in distutils-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-Versioneer provides two installation modes. The "classic" vendored mode installs
-a copy of versioneer into your repository. The experimental build-time dependency mode
-is intended to allow you to skip this step and simplify the process of upgrading.
-
-### Vendored mode
-
-* `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-   * Note that you will need to add `tomli; python_version < "3.11"` to your
-     build-time dependencies if you use `pyproject.toml`
-* run `versioneer install --vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
-
-### Build-time dependency mode
-
-* `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
-  to the `requires` key of the `build-system` table in `pyproject.toml`:
-  ```toml
-  [build-system]
-  requires = ["setuptools", "versioneer[toml]"]
-  build-backend = "setuptools.build_meta"
-  ```
-* run `versioneer install --no-vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
+* `pip install versioneer` to somewhere to your $PATH
+* add a `[versioneer]` section to your setup.cfg (see below)
+* run `versioneer install` in your source tree, commit the results
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -82,15 +57,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes).
+uncommitted changes.
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -187,45 +162,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/python-versioneer/python-versioneer/issues).
+[issues page](https://github.com/warner/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other languages) in subdirectories.
+  provide bindings to Python (and perhaps other langauges) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -245,28 +220,39 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
+### Unicode version strings
+
+While Versioneer works (and is continually tested) with both Python 2 and
+Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
+Newer releases probably generate unicode version strings on py2. It's not
+clear that this is wrong, but it may be surprising for applications when then
+write these strings to a network connection or include them in bytes-oriented
+APIs like cryptographic checksums.
+
+[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
+this question.
+
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg` and `pyproject.toml`, if necessary,
-  to include any new configuration settings indicated by the release notes.
-  See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install --[no-]vendor` in your source tree, to replace
+* edit `setup.cfg`, if necessary, to include any new configuration settings
+  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -275,263 +261,187 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
-## Similar projects
-
-* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
-  dependency
-* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
-  versioneer
-* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
-  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the "Unlicense", as described in
-https://unlicense.org/.
-
-[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
-[pypi-url]: https://pypi.python.org/pypi/versioneer/
-[travis-image]:
-https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
-[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
+Specifically, both are released under the Creative Commons "Public Domain
+Dedication" license (CC0-1.0), as described in
+https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
-# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
-# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
-# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
-# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
-# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-import configparser
+from __future__ import print_function
+try:
+    import configparser
+except ImportError:
+    import ConfigParser as configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
-from pathlib import Path
-from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
-from typing import NoReturn
-import functools
-
-have_tomllib = True
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    try:
-        import tomli as tomllib
-    except ImportError:
-        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
-    VCS: str
-    style: str
-    tag_prefix: str
-    versionfile_source: str
-    versionfile_build: Optional[str]
-    parentdir_prefix: Optional[str]
-    verbose: Optional[bool]
 
-
-def get_root() -> str:
+def get_root():
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
-    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (
-        os.path.exists(setup_py)
-        or os.path.exists(pyproject_toml)
-        or os.path.exists(versioneer_py)
-    ):
+    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
-        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (
-        os.path.exists(setup_py)
-        or os.path.exists(pyproject_toml)
-        or os.path.exists(versioneer_py)
-    ):
+    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         err = ("Versioneer was unable to run the project root directory. "
                "Versioneer requires setup.py to be executed from "
                "its immediate directory (like 'python setup.py COMMAND'), "
                "or in a way that lets it use sys.argv[0] to find the root "
                "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        my_path = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
+        me = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
+        if me_dir != vsr_dir:
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+                  % (os.path.dirname(me), versioneer_py))
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root: str) -> VersioneerConfig:
+def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise OSError (if setup.cfg is missing), or
+    # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    root_pth = Path(root)
-    pyproject_toml = root_pth / "pyproject.toml"
-    setup_cfg = root_pth / "setup.cfg"
-    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
-    if pyproject_toml.exists() and have_tomllib:
-        try:
-            with open(pyproject_toml, 'rb') as fobj:
-                pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
-        except (tomllib.TOMLDecodeError, KeyError) as e:
-            print(f"Failed to load config from {pyproject_toml}: {e}")
-            print("Try to load it from setup.cfg")
-    if not section:
-        parser = configparser.ConfigParser()
-        with open(setup_cfg) as cfg_file:
-            parser.read_file(cfg_file)
-        parser.get("versioneer", "VCS")  # raise error if missing
-
-        section = parser["versioneer"]
-
-    # `cast`` really shouldn't be used, but its simplest for the
-    # common VersioneerConfig users at the moment. We verify against
-    # `None` values elsewhere where it matters
-
+    setup_cfg = os.path.join(root, "setup.cfg")
+    parser = configparser.SafeConfigParser()
+    with open(setup_cfg, "r") as f:
+        parser.readfp(f)
+    VCS = parser.get("versioneer", "VCS")  # mandatory
+
+    def get(parser, name):
+        if parser.has_option("versioneer", name):
+            return parser.get("versioneer", name)
+        return None
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
-    cfg.style = section.get("style", "")
-    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
-    cfg.versionfile_build = section.get("versionfile_build")
-    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
-    if cfg.tag_prefix in ("''", '""', None):
+    cfg.VCS = VCS
+    cfg.style = get(parser, "style") or ""
+    cfg.versionfile_source = get(parser, "versionfile_source")
+    cfg.versionfile_build = get(parser, "versionfile_build")
+    cfg.tag_prefix = get(parser, "tag_prefix")
+    if cfg.tag_prefix in ("''", '""'):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = section.get("parentdir_prefix")
-    if isinstance(section, configparser.SectionProxy):
-        # Make sure configparser translates to bool
-        cfg.verbose = section.getboolean("verbose")
-    else:
-        cfg.verbose = section.get("verbose")
-
+    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
+    cfg.verbose = get(parser, "verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
+LONG_VERSION_PY = {}
+HANDLERS = {}
 
 
-def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
-    """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f: Callable) -> Callable:
+def register_vcs_handler(vcs, method):  # decorator
+    """Decorator to mark a method as the handler for a particular VCS."""
+    def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
-        HANDLERS.setdefault(vcs, {})[method] = f
+        if vcs not in HANDLERS:
+            HANDLERS[vcs] = {}
+        HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(
-    commands: List[str],
-    args: List[str],
-    cwd: Optional[str] = None,
-    verbose: bool = False,
-    hide_stderr: bool = False,
-    env: Optional[Dict[str, str]] = None,
-) -> Tuple[Optional[str], Optional[int]]:
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    process = None
-
-    popen_kwargs: Dict[str, Any] = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
-    for command in commands:
+    p = None
+    for c in commands:
         try:
-            dispcmd = str([command] + args)
+            dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
-        except OSError as e:
+        except EnvironmentError:
+            e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = process.communicate()[0].strip().decode()
-    if process.returncode != 0:
+    stdout = p.communicate()[0].strip()
+    if sys.version_info[0] >= 3:
+        stdout = stdout.decode()
+    if p.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, process.returncode
-    return stdout, process.returncode
+        return None, p.returncode
+    return stdout, p.returncode
 
 
-LONG_VERSION_PY['git'] = r'''
+LONG_VERSION_PY['git'] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain.
-# Generated by versioneer-0.29
-# https://github.com/python-versioneer/python-versioneer
+# This file is released into the public domain. Generated by
+# versioneer-0.18 (https://github.com/warner/python-versioneer)
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
-from typing import Any, Callable, Dict, List, Optional, Tuple
-import functools
 
 
-def get_keywords() -> Dict[str, str]:
+def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -539,23 +449,16 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
-    VCS: str
-    style: str
-    tag_prefix: str
-    parentdir_prefix: str
-    versionfile_source: str
-    verbose: bool
 
-
-def get_config() -> VersioneerConfig:
+def get_config():
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -565,187 +468,161 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
+LONG_VERSION_PY = {}
+HANDLERS = {}
 
 
-def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
-    """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f: Callable) -> Callable:
+def register_vcs_handler(vcs, method):  # decorator
+    """Decorator to mark a method as the handler for a particular VCS."""
+    def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(
-    commands: List[str],
-    args: List[str],
-    cwd: Optional[str] = None,
-    verbose: bool = False,
-    hide_stderr: bool = False,
-    env: Optional[Dict[str, str]] = None,
-) -> Tuple[Optional[str], Optional[int]]:
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    process = None
-
-    popen_kwargs: Dict[str, Any] = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
-    for command in commands:
+    p = None
+    for c in commands:
         try:
-            dispcmd = str([command] + args)
+            dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
-        except OSError as e:
+        except EnvironmentError:
+            e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = process.communicate()[0].strip().decode()
-    if process.returncode != 0:
+    stdout = p.communicate()[0].strip()
+    if sys.version_info[0] >= 3:
+        stdout = stdout.decode()
+    if p.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, process.returncode
-    return stdout, process.returncode
+        return None, p.returncode
+    return stdout, p.returncode
 
 
-def versions_from_parentdir(
-    parentdir_prefix: str,
-    root: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for _ in range(3):
+    for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        rootdirs.append(root)
-        root = os.path.dirname(root)  # up a level
+        else:
+            rootdirs.append(root)
+            root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
+def git_get_keywords(versionfile_abs):
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords: Dict[str, str] = {}
+    keywords = {}
     try:
-        with open(versionfile_abs, "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith("git_refnames ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["refnames"] = mo.group(1)
-                if line.strip().startswith("git_full ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["full"] = mo.group(1)
-                if line.strip().startswith("git_date ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["date"] = mo.group(1)
-    except OSError:
+        f = open(versionfile_abs, "r")
+        for line in f.readlines():
+            if line.strip().startswith("git_refnames ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["refnames"] = mo.group(1)
+            if line.strip().startswith("git_full ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["full"] = mo.group(1)
+            if line.strip().startswith("git_date ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["date"] = mo.group(1)
+        f.close()
+    except EnvironmentError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(
-    keywords: Dict[str, str],
-    tag_prefix: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if "refnames" not in keywords:
-        raise NotThisMethod("Short version file found")
+    if not keywords:
+        raise NotThisMethod("no keywords at all, weird")
     date = keywords.get("date")
     if date is not None:
-        # Use only the last line.  Previous lines may contain GPG signature
-        # information.
-        date = date.splitlines()[-1]
-
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
+    refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
-            # Filter out refs that exactly match prefix or that don't start
-            # with a number once the prefix is stripped (mostly a concern
-            # when prefix is '')
-            if not re.match(r'\d', r):
-                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -753,97 +630,52 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(
-    tag_prefix: str,
-    root: str,
-    verbose: bool,
-    runner: Callable = run_command
-) -> Dict[str, Any]:
+def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%%s*" %% tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces: Dict[str, Any] = {}
+    pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
-    # --abbrev-ref was added in git-1.6.3
-    if rc != 0 or branch_name is None:
-        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
-    branch_name = branch_name.strip()
-
-    if branch_name == "HEAD":
-        # If we aren't exactly on a branch, pick a branch which represents
-        # the current commit. If all else fails, we are on a branchless
-        # commit.
-        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
-        # --contains was added in git-1.5.4
-        if rc != 0 or branches is None:
-            raise NotThisMethod("'git branch --contains' returned error")
-        branches = branches.split("\n")
-
-        # Remove the first line if we're running detached
-        if "(" in branches[0]:
-            branches.pop(0)
-
-        # Strip off the leading "* " from the list of branches.
-        branches = [branch[2:] for branch in branches]
-        if "master" in branches:
-            branch_name = "master"
-        elif not branches:
-            branch_name = None
-        else:
-            # Pick the first branch that is returned. Good or bad.
-            branch_name = branches[0]
-
-    pieces["branch"] = branch_name
-
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -852,15 +684,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparsable. Maybe git-describe is misbehaving?
+            # unparseable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -877,35 +709,34 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
-    # Use only the last line.  Previous lines may contain GPG signature
-    # information.
-    date = date.splitlines()[-1]
+    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
+                       cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces: Dict[str, Any]) -> str:
+def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces: Dict[str, Any]) -> str:
+def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -922,79 +753,31 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
-
-    The ".dev0" means not master branch. Note that .dev0 sorts backwards
-    (a feature branch will appear "older" than the master branch).
+def render_pep440_pre(pieces):
+    """TAG[.post.devDISTANCE] -- No -dirty.
 
     Exceptions:
-    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
+    1: no tags. 0.post.devDISTANCE
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0"
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
-    """Split pep440 version string at the post-release segment.
-
-    Returns the release segments before the post-release and the
-    post-release version number (or -1 if no post-release segment is present).
-    """
-    vc = str.split(ver, ".post")
-    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
-
-
-def render_pep440_pre(pieces: Dict[str, Any]) -> str:
-    """TAG[.postN.devDISTANCE] -- No -dirty.
-
-    Exceptions:
-    1: no tags. 0.post0.devDISTANCE
-    """
-    if pieces["closest-tag"]:
         if pieces["distance"]:
-            # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
-            rendered = tag_version
-            if post_version is not None:
-                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
-            else:
-                rendered += ".post0.dev%%d" %% (pieces["distance"])
-        else:
-            # no commits, use the tag as the version
-            rendered = pieces["closest-tag"]
+            rendered += ".post.dev%%d" %% pieces["distance"]
     else:
         # exception #1
-        rendered = "0.post0.dev%%d" %% pieces["distance"]
+        rendered = "0.post.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces: Dict[str, Any]) -> str:
+def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1013,49 +796,20 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
-
-    The ".dev0" means not master branch.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%%d" %% pieces["distance"]
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%%s" %% pieces["short"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0.post%%d" %% pieces["distance"]
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+g%%s" %% pieces["short"]
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_old(pieces: Dict[str, Any]) -> str:
+def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Exceptions:
+    Eexceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -1064,15 +818,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces: Dict[str, Any]) -> str:
+def render_git_describe(pieces):
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1084,15 +838,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces: Dict[str, Any]) -> str:
+def render_git_describe_long(pieces):
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1104,51 +858,47 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
+def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
-    elif style == "pep440-branch":
-        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
-    elif style == "pep440-post-branch":
-        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions() -> Dict[str, Any]:
+def get_versions():
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -1161,15 +911,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for _ in cfg.versionfile_source.split('/'):
+        for i in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -1188,95 +938,83 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
+def git_get_keywords(versionfile_abs):
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords: Dict[str, str] = {}
+    keywords = {}
     try:
-        with open(versionfile_abs, "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith("git_refnames ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["refnames"] = mo.group(1)
-                if line.strip().startswith("git_full ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["full"] = mo.group(1)
-                if line.strip().startswith("git_date ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["date"] = mo.group(1)
-    except OSError:
+        f = open(versionfile_abs, "r")
+        for line in f.readlines():
+            if line.strip().startswith("git_refnames ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["refnames"] = mo.group(1)
+            if line.strip().startswith("git_full ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["full"] = mo.group(1)
+            if line.strip().startswith("git_date ="):
+                mo = re.search(r'=\s*"(.*)"', line)
+                if mo:
+                    keywords["date"] = mo.group(1)
+        f.close()
+    except EnvironmentError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(
-    keywords: Dict[str, str],
-    tag_prefix: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if "refnames" not in keywords:
-        raise NotThisMethod("Short version file found")
+    if not keywords:
+        raise NotThisMethod("no keywords at all, weird")
     date = keywords.get("date")
     if date is not None:
-        # Use only the last line.  Previous lines may contain GPG signature
-        # information.
-        date = date.splitlines()[-1]
-
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
+    refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
-            # Filter out refs that exactly match prefix or that don't start
-            # with a number once the prefix is stripped (mostly a concern
-            # when prefix is '')
-            if not re.match(r'\d', r):
-                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1284,97 +1022,52 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(
-    tag_prefix: str,
-    root: str,
-    verbose: bool,
-    runner: Callable = run_command
-) -> Dict[str, Any]:
+def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%s*" % tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces: Dict[str, Any] = {}
+    pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
-    # --abbrev-ref was added in git-1.6.3
-    if rc != 0 or branch_name is None:
-        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
-    branch_name = branch_name.strip()
-
-    if branch_name == "HEAD":
-        # If we aren't exactly on a branch, pick a branch which represents
-        # the current commit. If all else fails, we are on a branchless
-        # commit.
-        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
-        # --contains was added in git-1.5.4
-        if rc != 0 or branches is None:
-            raise NotThisMethod("'git branch --contains' returned error")
-        branches = branches.split("\n")
-
-        # Remove the first line if we're running detached
-        if "(" in branches[0]:
-            branches.pop(0)
-
-        # Strip off the leading "* " from the list of branches.
-        branches = [branch[2:] for branch in branches]
-        if "master" in branches:
-            branch_name = "master"
-        elif not branches:
-            branch_name = None
-        else:
-            # Pick the first branch that is returned. Good or bad.
-            branch_name = branches[0]
-
-    pieces["branch"] = branch_name
-
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1383,15 +1076,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparsable. Maybe git-describe is misbehaving?
+            # unparseable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1408,95 +1101,91 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
-    # Use only the last line.  Previous lines may contain GPG signature
-    # information.
-    date = date.splitlines()[-1]
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
+                       cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
+def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [versionfile_source]
+    files = [manifest_in, versionfile_source]
     if ipy:
         files.append(ipy)
-    if "VERSIONEER_PEP518" not in globals():
-        try:
-            my_path = __file__
-            if my_path.endswith((".pyc", ".pyo")):
-                my_path = os.path.splitext(my_path)[0] + ".py"
-            versioneer_file = os.path.relpath(my_path)
-        except NameError:
-            versioneer_file = "versioneer.py"
-        files.append(versioneer_file)
+    try:
+        me = __file__
+        if me.endswith(".pyc") or me.endswith(".pyo"):
+            me = os.path.splitext(me)[0] + ".py"
+        versioneer_file = os.path.relpath(me)
+    except NameError:
+        versioneer_file = "versioneer.py"
+    files.append(versioneer_file)
     present = False
     try:
-        with open(".gitattributes", "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith(versionfile_source):
-                    if "export-subst" in line.strip().split()[1:]:
-                        present = True
-                        break
-    except OSError:
+        f = open(".gitattributes", "r")
+        for line in f.readlines():
+            if line.strip().startswith(versionfile_source):
+                if "export-subst" in line.strip().split()[1:]:
+                    present = True
+        f.close()
+    except EnvironmentError:
         pass
     if not present:
-        with open(".gitattributes", "a+") as fobj:
-            fobj.write(f"{versionfile_source} export-subst\n")
+        f = open(".gitattributes", "a+")
+        f.write("%s export-subst\n" % versionfile_source)
+        f.close()
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(
-    parentdir_prefix: str,
-    root: str,
-    verbose: bool,
-) -> Dict[str, Any]:
+def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for _ in range(3):
+    for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        rootdirs.append(root)
-        root = os.path.dirname(root)  # up a level
+        else:
+            rootdirs.append(root)
+            root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.29) from
+# This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1505,49 +1194,50 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename: str) -> Dict[str, Any]:
+def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except OSError:
+    except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
+def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
+    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True,
                           indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces: Dict[str, Any]) -> str:
+def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces: Dict[str, Any]) -> str:
+def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1564,79 +1254,31 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
-
-    The ".dev0" means not master branch. Note that .dev0 sorts backwards
-    (a feature branch will appear "older" than the master branch).
+def render_pep440_pre(pieces):
+    """TAG[.post.devDISTANCE] -- No -dirty.
 
     Exceptions:
-    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
+    1: no tags. 0.post.devDISTANCE
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0"
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
-    """Split pep440 version string at the post-release segment.
-
-    Returns the release segments before the post-release and the
-    post-release version number (or -1 if no post-release segment is present).
-    """
-    vc = str.split(ver, ".post")
-    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
-
-
-def render_pep440_pre(pieces: Dict[str, Any]) -> str:
-    """TAG[.postN.devDISTANCE] -- No -dirty.
-
-    Exceptions:
-    1: no tags. 0.post0.devDISTANCE
-    """
-    if pieces["closest-tag"]:
         if pieces["distance"]:
-            # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
-            rendered = tag_version
-            if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
-            else:
-                rendered += ".post0.dev%d" % (pieces["distance"])
-        else:
-            # no commits, use the tag as the version
-            rendered = pieces["closest-tag"]
+            rendered += ".post.dev%d" % pieces["distance"]
     else:
         # exception #1
-        rendered = "0.post0.dev%d" % pieces["distance"]
+        rendered = "0.post.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces: Dict[str, Any]) -> str:
+def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1655,49 +1297,20 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
-    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
-
-    The ".dev0" means not master branch.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%s" % pieces["short"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+g%s" % pieces["short"]
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_old(pieces: Dict[str, Any]) -> str:
+def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Exceptions:
+    Eexceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1706,15 +1319,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces: Dict[str, Any]) -> str:
+def render_git_describe(pieces):
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1726,15 +1339,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces: Dict[str, Any]) -> str:
+def render_git_describe_long(pieces):
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1746,36 +1359,32 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
+def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
-    elif style == "pep440-branch":
-        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
-    elif style == "pep440-post-branch":
-        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1786,30 +1395,30 @@
             "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose: bool = False) -> Dict[str, Any]:
+def get_versions(verbose=False):
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
+    verbose = verbose or cfg.verbose
     assert cfg.versionfile_source is not None, \
         "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
@@ -1862,152 +1471,109 @@
         print("unable to compute version")
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
-def get_version() -> str:
+def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
-    """Get the custom setuptools subclasses used by Versioneer.
-
-    If the package uses a different cmdclass (e.g. one from numpy), it
-    should be provide as an argument.
-    """
+def get_cmdclass():
+    """Get the custom setuptools/distutils subclasses used by Versioneer."""
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
+        # Also see https://github.com/warner/python-versioneer/issues/52
 
-    cmds = {} if cmdclass is None else cmdclass.copy()
+    cmds = {}
 
-    # we add "version" to setuptools
-    from setuptools import Command
+    # we add "version" to both distutils and setuptools
+    from distutils.core import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options: List[Tuple[str, str, str]] = []
-        boolean_options: List[str] = []
+        user_options = []
+        boolean_options = []
 
-        def initialize_options(self) -> None:
+        def initialize_options(self):
             pass
 
-        def finalize_options(self) -> None:
+        def finalize_options(self):
             pass
 
-        def run(self) -> None:
+        def run(self):
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in setuptools
+    # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
-    # pip install -e . and setuptool/editable_wheel will invoke build_py
-    # but the build_py command is not expected to copy any files.
-
     # we override different "build_py" commands for both environments
-    if 'build_py' in cmds:
-        _build_py: Any = cmds['build_py']
-    else:
+    if "setuptools" in sys.modules:
         from setuptools.command.build_py import build_py as _build_py
+    else:
+        from distutils.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self) -> None:
+        def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
-            if getattr(self, "editable_mode", False):
-                # During editable installs `.py` and data files are
-                # not copied to build_lib
-                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
-    if 'build_ext' in cmds:
-        _build_ext: Any = cmds['build_ext']
-    else:
-        from setuptools.command.build_ext import build_ext as _build_ext
-
-    class cmd_build_ext(_build_ext):
-        def run(self) -> None:
-            root = get_root()
-            cfg = get_config_from_root(root)
-            versions = get_versions()
-            _build_ext.run(self)
-            if self.inplace:
-                # build_ext --inplace will only build extensions in
-                # build/lib<..> dir with no _version.py to write to.
-                # As in place builds will already have a _version.py
-                # in the module dir, we do not need to write one.
-                return
-            # now locate _version.py in the new build/ directory and replace
-            # it with an updated value
-            if not cfg.versionfile_build:
-                return
-            target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
-            if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
-                return
-            print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile, versions)
-    cmds["build_ext"] = cmd_build_ext
-
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
+        from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self) -> None:
+            def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -2023,20 +1589,20 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
+            from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
-            def run(self) -> None:
+            def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -2049,67 +1615,30 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
-    # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info: Any = cmds['egg_info']
-    else:
-        from setuptools.command.egg_info import egg_info as _egg_info
-
-    class cmd_egg_info(_egg_info):
-        def find_sources(self) -> None:
-            # egg_info.find_sources builds the manifest list and writes it
-            # in one shot
-            super().find_sources()
-
-            # Modify the filelist and normalize it
-            root = get_root()
-            cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
-            if cfg.versionfile_source:
-                # There are rare cases where versionfile_source might not be
-                # included by default, so we must be explicit
-                self.filelist.append(cfg.versionfile_source)
-            self.filelist.sort()
-            self.filelist.remove_duplicates()
-
-            # The write method is hidden in the manifest_maker instance that
-            # generated the filelist and was thrown away
-            # We will instead replicate their final normalization (to unicode,
-            # and POSIX-style paths)
-            from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
-
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
-
-    cmds['egg_info'] = cmd_egg_info
-
     # we override different "sdist" commands for both environments
-    if 'sdist' in cmds:
-        _sdist: Any = cmds['sdist']
-    else:
+    if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
+    else:
+        from distutils.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self) -> None:
+        def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
+        def make_release_tree(self, base_dir, files):
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -2154,34 +1683,29 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-OLD_SNIPPET = """
+INIT_PY_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
-INIT_PY_SNIPPET = """
-from . import {0}
-__version__ = {0}.get_versions()['version']
-"""
 
-
-def do_setup() -> int:
-    """Do main VCS-independent setup function for installing Versioneer."""
+def do_setup():
+    """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
+    except (EnvironmentError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (OSError, configparser.NoSectionError)):
+        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -2193,45 +1717,70 @@
                         "TAG_PREFIX": cfg.tag_prefix,
                         "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                         "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         })
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
-    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except OSError:
+        except EnvironmentError:
             old = ""
-        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
-        snippet = INIT_PY_SNIPPET.format(module)
-        if OLD_SNIPPET in old:
-            print(" replacing boilerplate in %s" % ipy)
-            with open(ipy, "w") as f:
-                f.write(old.replace(OLD_SNIPPET, snippet))
-        elif snippet not in old:
+        if INIT_PY_SNIPPET not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(snippet)
+                f.write(INIT_PY_SNIPPET)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        maybe_ipy = None
+        ipy = None
+
+    # Make sure both the top-level "versioneer.py" and versionfile_source
+    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
+    # they'll be copied into source distributions. Pip won't be able to
+    # install the package without this.
+    manifest_in = os.path.join(root, "MANIFEST.in")
+    simple_includes = set()
+    try:
+        with open(manifest_in, "r") as f:
+            for line in f:
+                if line.startswith("include "):
+                    for include in line.split()[1:]:
+                        simple_includes.add(include)
+    except EnvironmentError:
+        pass
+    # That doesn't cover everything MANIFEST.in can do
+    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
+    # it might give some false negatives. Appending redundant 'include'
+    # lines is safe, though.
+    if "versioneer.py" not in simple_includes:
+        print(" appending 'versioneer.py' to MANIFEST.in")
+        with open(manifest_in, "a") as f:
+            f.write("include versioneer.py\n")
+    else:
+        print(" 'versioneer.py' already in MANIFEST.in")
+    if cfg.versionfile_source not in simple_includes:
+        print(" appending versionfile_source ('%s') to MANIFEST.in" %
+              cfg.versionfile_source)
+        with open(manifest_in, "a") as f:
+            f.write("include %s\n" % cfg.versionfile_source)
+    else:
+        print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(cfg.versionfile_source, maybe_ipy)
+    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
     return 0
 
 
-def scan_setup_py() -> int:
+def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -2260,18 +1809,14 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
-def setup_command() -> NoReturn:
-    """Set up Versioneer and exit with appropriate error code."""
-    errors = do_setup()
-    errors += scan_setup_py()
-    sys.exit(1 if errors else 0)
-
-
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        setup_command()
+        errors = do_setup()
+        errors += scan_setup_py()
+        if errors:
+            sys.exit(1)
```

