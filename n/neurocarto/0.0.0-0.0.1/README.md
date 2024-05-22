# Comparing `tmp/neurocarto-0.0.0.tar.gz` & `tmp/neurocarto-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocarto-0.0.0.tar", last modified: Tue May 14 14:11:36 2024, max compression
+gzip compressed data, was "neurocarto-0.0.1.tar", last modified: Wed May 22 11:44:31 2024, max compression
```

## Comparing `neurocarto-0.0.0.tar` & `neurocarto-0.0.1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.574354 neurocarto-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-14 14:11:31.000000 neurocarto-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-14 14:11:36.574354 neurocarto-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 14:11:31.000000 neurocarto-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-14 14:11:31.000000 neurocarto-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 14:11:31.000000 neurocarto-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:11:36.574354 neurocarto-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.562354 neurocarto-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.562354 neurocarto-0.0.0/src/neurocarto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    26678 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/main_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/main_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.566354 neurocarto-0.0.0/src/neurocarto/probe_npx/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/desp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/npx.py
--rw-r--r--   0 runner    (1001) docker     (127)    25808 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/select_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/select_weaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/select_weaker_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/probe_npx/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.570354 neurocarto-0.0.0/src/neurocarto/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/_atlas_brain_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/atlas_brain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/atlas_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/atlas_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/bokeh_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/bokeh_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.570354 neurocarto-0.0.0/src/neurocarto/util/edit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/moving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/edit/surrounding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/probe_coor.py
--rw-r--r--   0 runner    (1001) docker     (127)    56943 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/util_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/util_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.574354 neurocarto-0.0.0/src/neurocarto/views/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25777 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    26266 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    22583 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/blueprint_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/data_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/image_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/image_plt.matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/image_plt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-14 14:11:31.000000 neurocarto-0.0.0/src/neurocarto/views/view_efficient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.574354 neurocarto-0.0.0/src/neurocarto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-14 14:11:36.000000 neurocarto-0.0.0/src/neurocarto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-14 14:11:36.000000 neurocarto-0.0.0/src/neurocarto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:11:36.000000 neurocarto-0.0.0/src/neurocarto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 14:11:36.000000 neurocarto-0.0.0/src/neurocarto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 14:11:36.000000 neurocarto-0.0.0/src/neurocarto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 14:11:36.000000 neurocarto-0.0.0/src/neurocarto.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:11:36.574354 neurocarto-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 14:11:31.000000 neurocarto-0.0.0/tests/test_electrode_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-14 14:11:31.000000 neurocarto-0.0.0/tests/test_npx_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-14 14:11:31.000000 neurocarto-0.0.0/tests/test_probe_oper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-14 14:11:31.000000 neurocarto-0.0.0/tests/test_util_blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-22 11:44:26.000000 neurocarto-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-22 11:44:31.464270 neurocarto-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-22 11:44:26.000000 neurocarto-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 11:44:26.000000 neurocarto-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:44:26.000000 neurocarto-0.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:44:31.464270 neurocarto-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.448269 neurocarto-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.452270 neurocarto-0.0.1/src/neurocarto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26678 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/main_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/main_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.456270 neurocarto-0.0.1/src/neurocarto/probe_npx/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/desp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/npx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25808 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/probe_npx/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.456270 neurocarto-0.0.1/src/neurocarto/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/_atlas_brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/atlas_brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/atlas_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/atlas_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/bokeh_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/bokeh_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.460270 neurocarto-0.0.1/src/neurocarto/util/edit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/moving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/edit/surrounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/probe_coor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59633 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/util_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/util_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/src/neurocarto/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26276 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22668 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/blueprint_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/data_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image_plt.matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/image_plt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 11:44:26.000000 neurocarto-0.0.1/src/neurocarto/views/view_efficient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/src/neurocarto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 11:44:31.000000 neurocarto-0.0.1/src/neurocarto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:44:31.464270 neurocarto-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_electrode_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_npx_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_probe_oper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-22 11:44:26.000000 neurocarto-0.0.1/tests/test_util_blueprint.py
```

### Comparing `neurocarto-0.0.0/LICENSE` & `neurocarto-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/PKG-INFO` & `neurocarto-0.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocarto
-Version: 0.0.0
+Version: 0.0.1
 Summary: A web-interface channelmap editor for Neuropixels probe familiy
 Author-email: Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, AntonioST
         
         Redistribution and use in source and binary forms, with or without
@@ -28,15 +28,15 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Homepage, https://github.com/AntonioST/NeuroCarto
-Project-URL: Documentation, https://github.com/AntonioST/NeuroCarto/wiki
+Project-URL: Documentation, https://neurocarto.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/AntonioST/NeuroCarto
 Project-URL: Issues, https://github.com/AntonioST/NeuroCarto/issues
 Keywords: Electrophysiology,Neuropixels,Channelmap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -57,14 +57,16 @@
 Requires-Dist: matplotlib
 Requires-Dist: typing_extensions
 Requires-Dist: bokeh
 
 NeuroCarto: A Neuropixels Channelmap Editor
 ===========================================
 
+[![PyPI - Version](https://img.shields.io/pypi/v/neurocarto)](https://pypi.org/project/neurocarto/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neurocarto)
 [![Documentation Status](https://readthedocs.org/projects/neurocarto/badge/?version=latest)](https://neurocarto.readthedocs.io/en/latest/?badge=latest)
 
 NeuroCarto is a neural probe channel map editor for the Neuropixels probe family.
 It allows user to create a blueprint for arranging electrodes in a desired density
 and generate a custom channel map.
 
 Features
@@ -92,16 +94,17 @@
 
 ### prepare environment.
 
 Require `Python 3.10`.
 
 ### Install
 
-
-This package will upload onto PyPI soon.
+```shell
+pip install neurocarto
+```
 
 ### Run
 
 ```shell
 neurocarto
 ```
```

### Comparing `neurocarto-0.0.0/README.md` & `neurocarto-0.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 NeuroCarto: A Neuropixels Channelmap Editor
 ===========================================
 
+[![PyPI - Version](https://img.shields.io/pypi/v/neurocarto)](https://pypi.org/project/neurocarto/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neurocarto)
 [![Documentation Status](https://readthedocs.org/projects/neurocarto/badge/?version=latest)](https://neurocarto.readthedocs.io/en/latest/?badge=latest)
 
 NeuroCarto is a neural probe channel map editor for the Neuropixels probe family.
 It allows user to create a blueprint for arranging electrodes in a desired density
 and generate a custom channel map.
 
 Features
@@ -32,16 +34,17 @@
 
 ### prepare environment.
 
 Require `Python 3.10`.
 
 ### Install
 
-
-This package will upload onto PyPI soon.
+```shell
+pip install neurocarto
+```
 
 ### Run
 
 ```shell
 neurocarto
 ```
```

### Comparing `neurocarto-0.0.0/pyproject.toml` & `neurocarto-0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 
 [project]
 name = 'neurocarto'
-version = '0.0.0'
+version = '0.0.1'
 authors = [
     { name = "Ta-Shun Su", email = "antoniost29@gmail.com" },
 ]
 description = "A web-interface channelmap editor for Neuropixels probe familiy"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
@@ -33,15 +33,15 @@
     "Typing :: Typed",
 ]
 
 dynamic = ["dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/AntonioST/NeuroCarto"
-Documentation = "https://github.com/AntonioST/NeuroCarto/wiki"
+Documentation = "https://neurocarto.readthedocs.io/en/latest/"
 Repository = "https://github.com/AntonioST/NeuroCarto"
 Issues = "https://github.com/AntonioST/NeuroCarto/issues"
 
 [project.scripts]
 neurocarto = "neurocarto.main_app:main"
 
 [tool.setuptools]
```

### Comparing `neurocarto-0.0.0/src/neurocarto/config.py` & `neurocarto-0.0.1/src/neurocarto/config.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/files.py` & `neurocarto-0.0.1/src/neurocarto/files.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/main_app.py` & `neurocarto-0.0.1/src/neurocarto/main_app.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/main_index.py` & `neurocarto-0.0.1/src/neurocarto/main_index.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe.py` & `neurocarto-0.0.1/src/neurocarto/probe.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/desp.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/desp.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             len([it for it in channelmap.electrodes if it.shank == s])
             for s in range(channelmap.probe_type.n_shank)
         ]
 
         ucs = ', '.join(map(lambda it: f's{it[0]}={it[1]}', enumerate(used_channel_on_shanks)))
 
         electrodes = npx_request_electrode(bp)
-        efficiency = npx_channel_efficiency(bp)
+        _, efficiency = npx_channel_efficiency(bp)
 
         return {
             'used channels': f'{used_channel}, total={channelmap.probe_type.n_channels}, ({ucs})',
             'request electrodes': f'{electrodes}',
             'channel efficiency': f'{100 * efficiency:.2f}%',
         }
```

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/io.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/io.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/npx.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/npx.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/plot.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/plot.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/select.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/select.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/select_default.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/select_default.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/select_weaker.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/select_weaker_debug.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/select_weaker_debug.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/stat.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,42 +68,48 @@
             case NpxProbeDesp.CATE_QUARTER:
                 electrode += count / 4
 
     return electrode
 
 
 @doc_link()
-def npx_channel_efficiency(bp: BlueprintFunctions, channelmap: ChannelMap = None, blueprint: NDArray[np.int_] = None) -> float:
+def npx_channel_efficiency(bp: BlueprintFunctions,
+                           channelmap: ChannelMap = None,
+                           blueprint: NDArray[np.int_] = None) -> tuple[float, float]:
     """
+    Calculate the area and channel efficiency for a channel map with a given blueprint.
 
     :param bp:
     :param channelmap: channelmap outcomes from *blueprint*
     :param blueprint: a given blueprint.
-    :return: channel efficiency value
+    :return: tuple of area and channel efficiency value
     """
     if channelmap is None:
         channelmap = bp.channelmap
 
     if blueprint is None:
         blueprint = bp._blueprint
 
     electrode = npx_request_electrode(bp, blueprint)
     channel = 0
+    excluded = 0
+    total = channelmap.probe_type.n_channels
 
     selected = blueprint[bp.selected_electrodes(channelmap)]
     for category, count in zip(*np.unique(selected, return_counts=True)):
         match category:
             case NpxProbeDesp.CATE_SET | NpxProbeDesp.CATE_FULL | NpxProbeDesp.CATE_HALF | NpxProbeDesp.CATE_QUARTER:
                 channel += count
             case NpxProbeDesp.CATE_EXCLUDED:
-                channel -= count
+                excluded += count
 
     ae = 0 if electrode == 0 else max(channel / electrode, 0)
     ce = 0 if ae == 0 else min(ae, 1 / ae)
-    return ce
+    ex = (total - excluded) / total
+    return ae, ce * ex
 
 
 class ElectrodeProbability(NamedTuple):
     sample_times: int
     """number of sample times"""
     summation: NDArray[np.int_]
     """summation matrix Array[count:int, S, C, R]"""
@@ -193,15 +199,15 @@
         for t in chmap.electrodes:
             mat[t.shank, t.column, t.row] += 1
 
         if probe.is_valid(chmap):
             complete += 1
 
         bp.set_blueprint(blueprint)
-        channel_efficiency.append(npx_channel_efficiency(bp))
+        channel_efficiency.append(npx_channel_efficiency(bp)[1])
 
     return ElectrodeProbability(sample_times, mat, complete, np.array(channel_efficiency))
 
 
 def _npx_electrode_probability_n(probe: NpxProbeDesp, chmap: ChannelMap, blueprint: list[NpxElectrodeDesp],
                                  selector: ElectrodeSelector,
                                  sample_times: int,
```

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/utils.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/utils.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/probe_npx/views.py` & `neurocarto-0.0.1/src/neurocarto/probe_npx/views.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/_atlas_brain_type.py` & `neurocarto-0.0.1/src/neurocarto/util/_atlas_brain_type.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/atlas_brain.py` & `neurocarto-0.0.1/src/neurocarto/util/atlas_brain.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/atlas_slice.py` & `neurocarto-0.0.1/src/neurocarto/util/atlas_slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.name = name
         """slice plane projection"""
 
         self.reference = reference
         """Image Array[uint, AP, DV, ML]"""
 
-        self.resolution = int(brain.resolution[get_args(SLICE).index(name)])
+        self.resolution = int(brain.resolution[get_args(SLICE).index(name)])  # FIXME change to (x,y,z)
         """um/pixel"""
 
         self.grid_y, self.grid_x = np.mgrid[0:self.height, 0:self.width]
 
     def __str__(self):
         return f'SliceView[{self.name}]'
 
@@ -311,14 +311,16 @@
             case _ if isinstance(c, np.ndarray):
                 if um:
                     c = np.round(c / self.resolution).astype(int)
                 plane, ax, ay = self.project(tuple(c))
             case _:
                 raise TypeError()
 
+        if plane < 0:
+            raise ValueError('negative plane index')
         return SlicePlane(plane, ax, ay, dw, dh, self)
 
 
 class CoronalView(SliceView):
 
     @property
     def n_plane(self) -> int:
@@ -413,15 +415,15 @@
     ax: int  # anchor x index
     ay: int  # anchor y index
     dw: int  # plane difference on left/right edge and the center
     dh: int  # plane difference on top/bottom edge and the center
     slice: SliceView
 
     @property
-    def slice_name(self) -> str:
+    def slice_name(self) -> SLICE:
         return self.slice.name
 
     @property
     def resolution(self) -> int:
         return self.slice.resolution
 
     @property
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/atlas_struct.py` & `neurocarto-0.0.1/src/neurocarto/util/atlas_struct.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,17 @@
                 if structure.id == item:
                     return structure
 
             raise KeyError(item)
         else:
             raise TypeError()
 
+    def __iter__(self) -> Iterator[Structure]:
+        return iter(self._structure.values())
+
     @property
     def regions(self) -> list[ACRONYM]:
         return list(self._structure)
 
     def alias(self, acronym: ACRONYM, *name: str):
         for it in name:
             self._structure[it] = self._structure[acronym]
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/bokeh_app.py` & `neurocarto-0.0.1/src/neurocarto/util/bokeh_app.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/bokeh_util.py` & `neurocarto-0.0.1/src/neurocarto/util/bokeh_util.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/debug.py` & `neurocarto-0.0.1/src/neurocarto/util/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,17 @@
     It is a debugging use function.
     """
 
     def __init__(self, disable=False):
         self.t = time.time()
         self.disable = disable
 
-    def reset(self):
+    def reset(self, message: str = None):
+        if message is not None and not self.disable:
+            print(message, '(reset)')
         self.t = time.time()
 
     def __call__(self, message: str = None) -> float:
         t = time.time()
         d = t - self.t
         self.t = t
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/_actions.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/_actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 import numpy as np
 
 from neurocarto.probe_npx import NpxProbeDesp, utils
 from neurocarto.util.edit.checking import use_probe, use_view
 from neurocarto.util.util_blueprint import BlueprintFunctions
 
@@ -129,71 +129,60 @@
     """
     bp.set_blueprint(bp.probe.load_blueprint(filename, bp.channelmap))
 
 
 @use_probe(NpxProbeDesp)
 def optimize_channelmap(bp: BlueprintFunctions, sample_times: int = 100, *,
                         single_process=False,
+                        n_worker: int = 1,
                         **kwargs):
     """
     Sample and find the optimized channelmap that has maxima channel efficiency.
 
     :param bp:
     :param sample_times: (int=100)
     :param single_process: (bool) debug use parameter
     :param kwargs: selector parameters
     """
     blueprint = bp.blueprint()
     if np.all(blueprint == bp.CATE_UNSET):
         bp.log_message('empty blueprint')
         return
 
-    _bp = bp.clone(pure=True)
+    from .optimize import optimize_channelmap as _optimize_channelmap
+
+    chmap = None
+    aeff = 0
+    ceff = 0
 
     if single_process:
-        chmap, ceff = _optimize_channelmap(_bp, sample_times, **kwargs)
+        chmap, aeff, ceff = _optimize_channelmap(bp, bp.channelmap, blueprint,
+                                                 sample_times=sample_times,
+                                                 **kwargs)
     else:
-        import multiprocessing
-        with multiprocessing.Pool(1) as pool:
-
-            job = pool.apply_async(_optimize_channelmap, (_bp, sample_times), kwargs)
-            pool.close()
+        import threading
 
-            while True:
-                try:
-                    chmap, ceff = job.get(0)
-                except multiprocessing.TimeoutError:
-                    yield 1
-                else:
-                    break
+        def target():
+            nonlocal chmap, aeff, ceff
+            chmap, aeff, ceff = _optimize_channelmap(bp, bp.channelmap, blueprint,
+                                                     sample_times=sample_times,
+                                                     n_worker=n_worker,
+                                                     **kwargs)
+
+        thread = threading.Thread(target=target, daemon=True)
+        thread.start()
+
+        while thread.is_alive():
+            yield 1
+        thread.join()
 
-    bp.set_status_line(f'finished. got max(Ceff)={100 * ceff:.2f}%')
+    bp.set_status_line(f'finished. got max(Ceff)={100 * ceff:.2f}% and Aeff={100 * aeff:.2f}')
     bp.set_channelmap(chmap)
 
 
-def _optimize_channelmap(bp: BlueprintFunctions, sample_times: int = 100, **kwargs):
-    from neurocarto.probe_npx.npx import ChannelMap
-    from neurocarto.probe_npx.stat import npx_channel_efficiency
-
-    blueprint_arr = bp.blueprint()
-    blueprint_lst = bp.apply_blueprint(blueprint=blueprint_arr)
-
-    chmap: ChannelMap = bp.channelmap
-    ceff = npx_channel_efficiency(bp, chmap, blueprint_arr)
-    max_chmap = (chmap, ceff)
-
-    for i in range(sample_times):
-        chmap = bp.select_electrodes(chmap, blueprint_lst, **kwargs)
-        ceff = npx_channel_efficiency(bp, chmap, blueprint_arr)
-        if ceff > max_chmap[1]:
-            max_chmap = (chmap, ceff)
-
-    return max_chmap
-
-
 @use_view('AtlasBrainView')
 def atlas_label(bp: BlueprintFunctions, *args, color='cyan'):
     """
     Set labels on atlas brain image.
 
     commands:
     * clear : clear labels
@@ -343,14 +332,15 @@
     :param color: label color
     """
     if ap is None and ml is None:
         if (coor := bp.atlas_current_probe(shank, ref)) is None:
             bp.log_message('fail to figure current probe coordinate')
             return
 
+        assert coor.bregma is not None
         bp.set_script_input(
             None,
             f'{coor.x / 1000:.1f}',
             f'{coor.z / 1000:.1f}',
             f'{coor.y / 1000:.1f}' if coor.y != 0 else None,
             f'shank={coor.s}',
             f'rx={coor.rx:.0f}' if coor.rx != 0 else None,
@@ -366,14 +356,41 @@
 
         bp.atlas_set_anchor_on_probe(coor)
 
         if label is not None:
             bp.atlas_add_label(label, (ap, dv, ml), origin=ref, color=color)
 
 
+@use_view('AtlasBrainView')
+def highlight_electrode_inside_region(bp: BlueprintFunctions,
+                                      region: str,
+                                      mode: Literal['replace', 'append', 'exclude'] = 'replace'):
+    """
+    Capture electrodes inside a region.
+
+    :param bp:
+    :param region: (str) region ID, acronym or its partial description
+    :param mode: (one of 'replace', 'append' or 'exclude') capture mode
+    """
+    if (region := bp.atlas_get_region_name(name := region)) is None:
+        bp.log_message(f'region "{name}" not found')
+        return
+
+    try:
+        mask = bp.atlas_mask_region(region)
+    except BaseException as e:
+        bp.log_message(repr(e))
+        return
+
+    if np.count_nonzero(mask) == 0:
+        bp.log_message(f'no electrode inside "{region}"')
+    else:
+        bp.capture_electrode(mask, mode=mode)
+
+
 @use_probe(NpxProbeDesp, create=False)
 def blueprint_simple_init_script_from_activity_data_with_a_threshold(bp: BlueprintFunctions, filename: str, threshold: float):
     """
     Initial a blueprint based on the experimental activity data with a given threshold,
     which follows:
 
     * set NaN area as excluded zone.
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/actions.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/actions.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/atlas.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/atlas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,270 @@
 from __future__ import annotations
 
 import textwrap
 from typing import TYPE_CHECKING
 
 import numpy as np
+from numpy.typing import NDArray
 
 from neurocarto.util import probe_coor
 from neurocarto.util.util_blueprint import BlueprintFunctions
 from neurocarto.util.utils import SPHINX_BUILD, doc_link
 from neurocarto.views.base import ControllerView
 
 if TYPE_CHECKING:
     from neurocarto.views.atlas import AtlasBrainView, Label
+    from neurocarto.util.atlas_struct import Structure
 elif SPHINX_BUILD:
     Label = 'neurocarto.views.atlas.Label'
+    Structure = 'neurocarto.util.atlas_struct.Structure'
 
 __all__ = [
+    'atlas_get_region_name',
+    'atlas_get_region',
     'atlas_get_slice',
     'atlas_set_slice',
     'atlas_add_label',
     'atlas_get_label',
     'atlas_focus_label',
     'atlas_del_label',
     'atlas_clear_labels',
     'atlas_set_transform',
     'atlas_set_anchor',
     'atlas_new_probe',
     'atlas_current_probe',
     'atlas_set_anchor_on_probe',
+    'atlas_coor_electrode',
+    'atlas_mask_region',
 ]
 
 
+def _get_atlas(controller: ControllerView | AtlasBrainView) -> AtlasBrainView | None:
+    from neurocarto.views.atlas import AtlasBrainView
+    if isinstance(controller, ControllerView):
+        return controller.get_view(AtlasBrainView)
+    elif isinstance(controller, AtlasBrainView):
+        return controller
+    else:
+        raise TypeError()
+
+
+@doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_get_region_name.__doc__))
+def atlas_get_region_name(controller: ControllerView | AtlasBrainView, region: int | str) -> str | None:
+    """
+    {DOC}
+    :see: {BlueprintFunctions#atlas_get_region_name()}
+    """
+    if (structure := atlas_get_region(controller, region)) is not None:
+        return structure.acronym
+    return None
+
+
+def atlas_get_region(controller: ControllerView | AtlasBrainView, region: int | str) -> Structure | None:
+    if (atlas := _get_atlas(controller)) is None:
+        return None
+
+    try:
+        structure = atlas._structure
+    except:
+        from neurocarto.util.atlas_struct import Structures
+        structure = Structures.of(atlas.brain)
+
+    try:
+        return structure[region]
+    except KeyError:
+        pass
+
+    if isinstance(region, int):
+        return None
+
+    region = region.lower()
+    for s in structure:
+        if s.acronym.lower().startswith(region):
+            return s
+        if s.name.lower().startswith(region):
+            return s
+    return None
+
+
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_get_slice.__doc__))
-def atlas_get_slice(controller: ControllerView, *, um=False) -> tuple[str | None, int | None]:
+def atlas_get_slice(controller: ControllerView | AtlasBrainView, *, um=False) -> tuple[str | None, int | None]:
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_get_slice()}
     """
-    atlas: AtlasBrainView
-    if (atlas := controller.get_view('AtlasBrainView')) is None:  # type: ignore[assignment]
+    if (atlas := _get_atlas(controller)) is None:
         return None, None
 
     name = atlas.brain_view.name
     if (plane := atlas.brain_slice) is None:
         return name, None
 
     index = plane.plane
     if um:
         index = atlas.get_plane_offset(index)
 
     return name, index
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_set_slice.__doc__))
-def atlas_set_slice(controller: ControllerView,
+def atlas_set_slice(controller: ControllerView | AtlasBrainView,
                     view: str = None,
                     plane: int = None, *, um=False):
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_set_slice()}
     """
-    atlas: AtlasBrainView
-    if (atlas := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (atlas := _get_atlas(controller)) is not None:
         if view is not None:
             atlas.update_brain_view(view)
 
         if plane is not None:
             if um:
                 plane = atlas.get_plane_index(plane)
 
             atlas.update_brain_slice(plane)
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_add_label.__doc__))
-def atlas_add_label(controller: ControllerView, text: str,
+def atlas_add_label(controller: ControllerView | AtlasBrainView,
+                    text: str,
                     pos: tuple[float, float] | tuple[float, float, float], *,
                     origin: str = 'bregma', color: str = 'cyan', replace=True) -> Label | None:
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_add_label()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is not None:
         return view.add_label(text, pos, origin=origin, color=color, replace=replace)
     return None
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_get_label.__doc__))
-def atlas_get_label(controller: ControllerView, index: int | str) -> Label | None:
+def atlas_get_label(controller: ControllerView | AtlasBrainView,
+                    index: int | str) -> Label | None:
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_get_label()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is not None:
         if isinstance(index, str):
             if (index := view.index_label(index)) is None:
                 return None
 
         try:
             return view.get_label(index)
         except IndexError:
             pass
 
     return None
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_focus_label.__doc__))
-def atlas_focus_label(controller: ControllerView, label: int | str | Label):
+def atlas_focus_label(controller: ControllerView | AtlasBrainView,
+                      label: int | str | Label):
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_focus_label()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is not None:
         view.focus_label(label)
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_del_label.__doc__))
-def atlas_del_label(controller: ControllerView, i: int | str | Label | list[int | str | Label]):
+def atlas_del_label(controller: ControllerView | AtlasBrainView,
+                    i: int | str | Label | list[int | str | Label]):
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_del_label()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is not None:
         view.del_label(i)
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_clear_labels.__doc__))
-def atlas_clear_labels(controller: ControllerView):
+def atlas_clear_labels(controller: ControllerView | AtlasBrainView):
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_clear_labels()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is not None:
         view.clear_labels()
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_set_transform.__doc__))
-def atlas_set_transform(controller: ControllerView,
+def atlas_set_transform(controller: ControllerView | AtlasBrainView,
                         p: tuple[float, float] = None,
                         s: float | tuple[float, float] = None,
                         rt: float = None):
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_set_transform()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is not None:
         view.update_boundary_transform(p=p, s=s, rt=rt)
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_set_anchor.__doc__))
-def atlas_set_anchor(controller: ControllerView,
+def atlas_set_anchor(controller: ControllerView | AtlasBrainView,
                      p: tuple[float, float],
                      a: tuple[float, float] = (0, 0)):
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_set_anchor()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is not None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is not None:
         view.set_anchor_to(p, a)
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_new_probe.__doc__))
-def atlas_new_probe(controller: ControllerView,
+def atlas_new_probe(controller: ControllerView | AtlasBrainView,
                     ap: float, dv: float, ml: float,
                     shank: int = 0,
                     rx: float = 0, ry: float = 0, rz: float = 0,
                     depth: float = 0,
                     ref: str = 'bregma') -> probe_coor.ProbeCoordinate | None:
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_new_probe()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is None:
         return None
 
+    from neurocarto.util.atlas_brain import REFERENCE
+    origin = REFERENCE[ref][view.brain_view.brain.atlas_name]
+
     # get probe coordinate instance
-    name = view.brain_view.brain.atlas_name
-    return probe_coor.ProbeCoordinate.from_bregma(name, ap, dv, ml, s=shank, rx=rx, ry=ry, rz=rz, depth=depth, ref=ref)
+    return probe_coor.ProbeCoordinate(ap, dv, ml, shank, rx, ry, rz, depth, origin)
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_current_probe.__doc__))
 def atlas_current_probe(bp: BlueprintFunctions,
-                        controller: ControllerView,
+                        controller: ControllerView | AtlasBrainView,
                         shank: int = 0,
                         ref: str = 'bregma') -> probe_coor.ProbeCoordinate | None:
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_current_probe()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is None:
         return None
 
     from neurocarto.util.atlas_brain import REFERENCE
 
     brain = view.brain_slice
     try:
         origin = REFERENCE[ref][brain.slice.brain.atlas_name]
     except KeyError:
         return None
 
     transform = view.get_boundary_state()
     a, a_ = probe_coor.prepare_affine_matrix_both(**transform)
 
-    s = bp.s == shank
-    p = np.vstack([
-        bp.x[s],
-        bp.y[s],
-        np.ones((np.count_nonzero(s),)),
-    ])  # Array[float, (x,y,1), N']
+    p = _electrode_coor(bp, bp.s == shank)  # Array[float, (x,y,1), N']
     q = probe_coor.project_i2b(origin, brain, a_ @ p)  # Array[float, (ap,dv,ml), N']
 
     i = np.argmin(np.abs(q[1]))
     ap, dv, ml = q[:, i]
     depth = np.max(q[1])
 
     # set slice rotation
@@ -230,27 +275,26 @@
         case 'sagittal':
             rot[2] = transform['rt']
         case 'transverse':
             rot[1] = -transform['rt']
         case _:
             raise RuntimeError('un-reachable')
 
-    return probe_coor.ProbeCoordinate(ap, 0, ml, shank, rot[0], rot[1], rot[2], depth)
+    return probe_coor.ProbeCoordinate(ap, 0, ml, shank, rot[0], rot[1], rot[2], depth, origin)
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_set_anchor_on_probe.__doc__))
 def atlas_set_anchor_on_probe(bp: BlueprintFunctions,
-                              controller: ControllerView,
+                              controller: ControllerView | AtlasBrainView,
                               coor: probe_coor.ProbeCoordinate):
     """
     {DOC}
     :see: {BlueprintFunctions#atlas_set_anchor_on_probe()}
     """
-    view: AtlasBrainView
-    if (view := controller.get_view('AtlasBrainView')) is None:  # type: ignore[assignment]
+    if (view := _get_atlas(controller)) is None:
         return
 
     # set brain slice to corresponding plane
     brain_slice = probe_coor.get_plane_at(view.brain_view, coor)
     view.update_brain_slice(brain_slice, update_image=False)
 
     # set slice rotation
@@ -266,25 +310,118 @@
 
     view.update_boundary_transform(rt=rot)
 
     # another slice on to probe
     if bp.channelmap is None:
         ex = ey = 0
     else:
-        electrode_s = bp.s == coor.s
-        electrode_x = bp.x[electrode_s]  # Array[um:float, N]
-        electrode_y = bp.y[electrode_s]  # Array[um:float, N]
+        electrode = _electrode_coor(bp, bp.s == coor.s)  # Array[um:float, (x, y, 1), N]
 
         from neurocarto.util.util_numpy import closest_point_index
-        if (i := closest_point_index(electrode_y, coor.depth, bp.dy * 2)) is not None:
-            ex = electrode_x[i]
+        if (i := closest_point_index(electrode[1], coor.depth, bp.dy * 2)) is not None:
+            ex = electrode[0, i]
         else:
             # cannot find nearest electrode position
             ex = 0
 
         ey = coor.depth
 
     cx = brain_slice.width / 2
     cy = brain_slice.height / 2
     ax = brain_slice.ax * brain_slice.resolution - cx
     ay = cy - brain_slice.ay * brain_slice.resolution
     view.set_anchor_to((ex, ey), (ax, ay))
+
+
+@doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_coor_electrode.__doc__))
+def atlas_coor_electrode(bp: BlueprintFunctions,
+                         controller: ControllerView | AtlasBrainView,
+                         coor: probe_coor.ProbeCoordinate = None,
+                         electrode: NDArray[np.int_] | NDArray[np.bool_] | NDArray[np.float_] = None,
+                         bregma: str | None = 'bregma') -> NDArray[np.float_]:
+    """
+    {DOC}
+    :see: {BlueprintFunctions#atlas_coor_electrode()}
+    """
+    if (view := _get_atlas(controller)) is None:
+        raise RuntimeError('cannot determine current atlas')
+
+    if coor is None:
+        if (coor := atlas_current_probe(bp, view)) is None:
+            raise RuntimeError('Cannot determine current probe coordinate.')
+
+    if bregma is not None:
+        from neurocarto.util.atlas_brain import REFERENCE
+        origin = REFERENCE[bregma][view.brain.atlas_name]
+    else:
+        origin = None
+
+    a, a_ = probe_coor.prepare_affine_matrix_both(**view.get_boundary_state())
+    p = _electrode_coor(bp, electrode)  # Array[um:float, (x, y, 1), N] probe-origin
+    q = probe_coor.project_i2b(origin, probe_coor.get_plane_at(view.brain_view, coor), a_ @ p)
+    return q.T  # Array[um:float, N, (ap, dv, ml)] bregma-origin
+
+
+@doc_link(DOC=textwrap.dedent(BlueprintFunctions.atlas_mask_region.__doc__))
+def atlas_mask_region(bp: BlueprintFunctions,
+                      controller: ControllerView | AtlasBrainView,
+                      region: str,
+                      coor: probe_coor.ProbeCoordinate = None,
+                      electrode: NDArray[np.int_] | NDArray[np.bool_] | NDArray[np.float_] = None) -> NDArray[np.bool_]:
+    """
+    {DOC}
+    :see: {BlueprintFunctions#atlas_mask_region()}
+    """
+    if (view := _get_atlas(controller)) is None:
+        raise RuntimeError('cannot determine current atlas')
+
+    if coor is None:
+        if (coor := atlas_current_probe(bp, view)) is None:
+            raise RuntimeError('Cannot determine current probe coordinate.')
+
+    p = atlas_coor_electrode(bp, view, coor, electrode, bregma=None)  # Array[um:float, N, (ap, dv, ml)] atlas-origin
+    q = (p / view.brain.resolution).astype(int)  # Array[index:int, N, (ap, dv, ml)]
+    r = view.brain.annotation[tuple(q.T)]  # Array[annotation:int, N]
+
+    try:
+        structure = view._structure
+    except:
+        from neurocarto.util.atlas_struct import Structures
+        structure = Structures.of(view.brain)
+
+    ret = np.zeros_like(r, dtype=bool)
+    if (target := atlas_get_region(view, region)) is None:
+        return ret
+
+    for sub in structure.iter_subregions(target):
+        np.logical_or(ret, r == sub.id, out=ret)
+    return ret
+
+
+def _electrode_coor(bp: BlueprintFunctions,
+                    electrode: NDArray[np.int_] | NDArray[np.bool_] | NDArray[np.float_] = None) -> NDArray[np.float_]:
+    """
+
+    :param bp:
+    :param electrode: electrode index (Array[int, N]), mask (Array[bool, E]) or position (Array[um:float, N, (x, y)])
+    :return: electrode position on probe Array[um:float, (x, y, 1), N]
+    """
+    if electrode is None:
+        return np.vstack([
+            bp.x,
+            bp.y,
+            np.ones((len(bp.x),))
+        ])  # Array[float, (x,y,1), N]
+    elif electrode.ndim == 1:
+        return np.vstack([
+            (x := bp.x[electrode]),
+            bp.y[electrode],
+            np.ones((len(x),))
+        ])
+    elif electrode.ndim == 2:
+        return np.vstack([
+            electrode[:, 0],
+            electrode[:, 1],
+            np.ones((len(electrode),))
+        ])
+    else:
+        raise ValueError('wrong electrode position dimension')
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/category.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/category.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/checking.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/checking.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/clustering.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/clustering.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/data.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/data.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/debug.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/debug.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/moving.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/moving.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/plot.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/plot.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/probe.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/probe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import textwrap
-from typing import Any
+from typing import Any, Literal
 
 import numpy as np
 from numpy.typing import NDArray
 
 from neurocarto.probe import ProbeDesp, ElectrodeDesp, M
 from neurocarto.util.util_blueprint import BlueprintFunctions
 from neurocarto.util.utils import SPHINX_BUILD, doc_link
@@ -35,21 +35,35 @@
     app.on_new(code)
     return app.probe_view.channelmap
 
 
 @doc_link(DOC=textwrap.dedent(BlueprintFunctions.capture_electrode.__doc__))
 def capture_electrode(self: BlueprintFunctions, controller: ControllerView,
                       index: NDArray[np.int_] | NDArray[np.bool_],
-                      state: list[int] = None):
+                      state: list[int] = None,
+                      mode: Literal['replace', 'append', 'exclude'] = 'replace'):
     """
     {DOC}
     :see: {BlueprintFunctions#capture_electrode()}
     """
     electrodes = self.electrodes
-    captured = [electrodes[int(it)] for it in np.arange(len(self.s))[index]]
+    captured = set([int(it) for it in np.arange(len(self.s))[index]])
+    previous = set([int(it) for it in captured_electrodes(controller, all=True)])
+
+    match mode:
+        case 'replace':
+            pass
+        case 'append':
+            captured.update(previous)
+        case 'exclude':
+            captured = previous.difference(captured)
+        case _:
+            raise ValueError(f'unknown mode "{mode}"')
+
+    captured = [electrodes[it] for it in captured]
 
     view = controller.get_app().probe_view
     if state is None:
         view.set_captured_electrodes(captured)
     else:
         for s in state:
             try:
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/script.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/script.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/edit/surrounding.py` & `neurocarto-0.0.1/src/neurocarto/util/edit/surrounding.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/probe_coor.py` & `neurocarto-0.0.1/src/neurocarto/util/probe_coor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import sys
-from typing import NamedTuple
+from typing import NamedTuple, overload
 
 import numpy as np
 from numpy.typing import NDArray
 
 from neurocarto.util.atlas_slice import SliceView, SlicePlane
 
 if sys.version_info >= (3, 11):
@@ -40,37 +40,66 @@
     """shank s y-axis (dv) rotate degree"""
     rz: float = 0
     """shank s z-axis (ml) rotate degree"""
 
     depth: float = 0
     """shank s insert depth (um)"""
 
-    @classmethod
-    def from_bregma(cls, atlas_name: str, ap: float, dv: float, ml: float, ref: str = 'bregma', **kwargs) -> Self:
+    bregma: tuple[float, float, float] | None = None
+    """bregma coordinate (ap, dv, ml)"""
+
+    def to_origin(self) -> Self:
+        """
+        move coordinate to atlas-origin.
         """
+        if self.bregma is None:
+            return self
 
-        :param atlas_name: atlas brain name
-        :param ap: um
-        :param dv: um
-        :param ml: um
-        :param ref: reference origin, default use 'bregma'
-        :param kwargs: {ProbeCoordinate}'s other parameters.
-        :return:
-        :raises KeyError:
+        return self._replace(
+            x=self.bregma[0] - self.x,
+            y=self.bregma[1] + self.y,
+            z=self.bregma[2] + self.z,
+            bregma=None
+        )
+
+    @overload
+    def to_bregma(self, atlas_name: tuple[float, float, float]) -> Self:
+        pass
+
+    @overload
+    def to_bregma(self, atlas_name: str, ref: str = 'bregma') -> Self:
+        pass
+
+    def to_bregma(self, atlas_name, ref: str = 'bregma') -> Self:
         """
-        from neurocarto.util.atlas_brain import REFERENCE
-        bregma = REFERENCE[ref][atlas_name]
+        move coordinate to bregma-origin.
 
-        x = bregma[0] - ap
-        y = bregma[1] + dv
-        z = bregma[2] + ml
-        return ProbeCoordinate(x, y, z, **kwargs)  # type: ignore[return-value]
+        :param atlas_name: atlas name
+        :param ref:
+        :return:
+        """
+        match atlas_name:
+            case str():
+                from neurocarto.util.atlas_brain import REFERENCE
+                bregma = REFERENCE[ref][atlas_name]
+            case (int() | float(), int() | float(), int() | float()):
+                bregma = atlas_name
+            case _:
+                raise TypeError()
+
+        return self.to_origin()._replace(
+            x=bregma[0] - self.x,
+            y=self.y - bregma[1],
+            z=self.z - bregma[2],
+            bregma=bregma
+        )
 
 
 def get_plane_at(view: SliceView, pc: ProbeCoordinate) -> SlicePlane:
+    pc = pc.to_origin()
     a = np.deg2rad([pc.rx, pc.ry, pc.rz])
     dw, dh = view.angle_offset(tuple(a))
     return view.plane_at((pc.x, pc.y, pc.z), um=True).with_offset(dw, dh)
 
 
 def prepare_affine_matrix(dx: float, dy: float, sx: float, sy: float, rt: float) -> NDArray[np.float_]:
     r"""
@@ -174,15 +203,17 @@
             return (a @ q)[[0, 1], :]
         case (3, n):
             return a @ p
         case _:
             raise ValueError()
 
 
-def project_b2i(bregma: tuple[float, float, float], view: SlicePlane, p: NDArray[np.float_], *,
+def project_b2i(bregma: tuple[float, float, float] | None,
+                view: SlicePlane,
+                p: NDArray[np.float_], *,
                 keep_plane: bool = False) -> NDArray[np.float_]:
     """
     project coordinate from bregma-origin to image-origin.
 
     :param bregma: bregma (ap, dv, ml) in um
     :param view: projection view
     :param p: Array[float, (ap, dv, ml) [,N]] position in um
@@ -197,30 +228,33 @@
             q = np.empty((3, n), dtype=float)
         case _:
             raise ValueError()
 
     cx = view.width / 2
     cy = view.height / 2
 
-    q[0] = bregma[0] - p[0]
-    q[1] = p[1] + bregma[1]
-    q[2] = p[2] + bregma[2]
+    if bregma is not None:
+        q[0] = bregma[0] - p[0]
+        q[1] = p[1] + bregma[1]
+        q[2] = p[2] + bregma[2]
+    else:
+        q[:] = p
 
     q = q[view.slice.project_index, :]
     q = q[[1, 2, 0], :]
 
     q[0] = q[0] - cx
     q[1] = cy - q[1]
     if not keep_plane:
         q[2] = 1
 
     return q
 
 
-def project_i2b(bregma: tuple[float, float, float], view: SlicePlane, p: NDArray[np.float_]) -> NDArray[np.float_]:
+def project_i2b(bregma: tuple[float, float, float] | None, view: SlicePlane, p: NDArray[np.float_]) -> NDArray[np.float_]:
     """
     project coordinate from image-origin to bregma-origin.
 
     :param bregma: bregma (ap, dv, ml) in um
     :param view: projection view
     :param p: Array[float, (x,y[,1]) [,N]] position in um
     :return: Array[float, (ap, dv, ml) [,N]] transform position in um
@@ -233,20 +267,21 @@
             q = np.empty((3, n), dtype=float)
         case _:
             raise ValueError()
 
     cx = view.width / 2
     cy = view.height / 2
 
-    x = p[0] + cx
-    y = cy - p[1]
+    x = p[0] + cx  # x position to image-corner
+    y = cy - p[1]  # y position to image-corner
 
     pi, xi, yi = view.slice.project_index
     q[xi] = x
     q[yi] = y
     q[pi] = view.plane_idx_at(x, y, um=True) * view.resolution
 
-    q[0] = bregma[0] - q[0]
-    q[1] -= bregma[1]
-    q[2] -= bregma[2]
+    if bregma is not None:
+        q[0] = bregma[0] - q[0]
+        q[1] -= bregma[1]
+        q[2] -= bregma[2]
 
     return q
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/util_blueprint.py` & `neurocarto-0.0.1/src/neurocarto/util/util_blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import functools
 import sys
 from collections.abc import Callable, Sequence
 from pathlib import Path
-from typing import TYPE_CHECKING, overload, Generic, Final, Any
+from typing import TYPE_CHECKING, overload, Generic, Final, Any, Literal
 
 import numpy as np
 from numpy.typing import NDArray
 
 from neurocarto.probe import ProbeDesp, M, E, get_probe_desp
 from neurocarto.util.edit.checking import use_probe
 from neurocarto.util.utils import doc_link, SPHINX_BUILD
@@ -179,23 +179,26 @@
     **Atlas Brain image view functions**
 
     Call methods from {AtlasBrainView}.
 
     .. hlist::
         :columns: 2
 
+        * {#atlas_get_region_name()}
         * {#atlas_set_slice()}
         * {#atlas_add_label()}
         * {#atlas_add_label()}
         * {#atlas_del_label()}
         * {#atlas_clear_labels()}
         * {#atlas_set_transform()}
         * {#atlas_set_anchor()}
         * {#atlas_new_probe()}
         * {#atlas_set_anchor_on_probe()}
+        * {#atlas_coor_electrode()}
+        * {#atlas_mask_region()}
 
     **Blueprint script view functions**
 
     Call methods from {BlueprintScriptView}.
 
     .. hlist::
         :columns: 2
@@ -276,16 +279,20 @@
             electrodes = []
 
         self.electrodes: Final[list[E]] = electrodes
         """all available electrodes"""
 
         if chmap is not None:
             self.s: Final[NDArray[np.int_]] = np.array([it.s for it in self.electrodes])
+            """shank"""
             self.x: Final[NDArray[np.int_]] = np.array([it.x for it in self.electrodes])
+            """x position in um"""
             self.y: Final[NDArray[np.int_]] = np.array([it.y for it in self.electrodes])
+            """y position in um"""
+
             self.dx: Final[float] = float(np.min(np.diff(np.unique(self.x))))
             self.dy: Final[float] = float(np.min(np.diff(np.unique(self.y))))
             if self.dx <= 0 or self.dy <= 0:
                 raise ValueError(f'dx={self.dx}, dy={self.dy}')
 
             self._position_index: dict[tuple[int, int, int], int] = {
                 (int(self.s[i]), int(self.x[i] / self.dx), int(self.y[i] / self.dy)): i
@@ -1252,25 +1259,27 @@
         if (controller := self._controller) is not None:
             return new_channelmap(controller, code)
         else:
             raise RuntimeError()
 
     @doc_link()
     def capture_electrode(self, index: NDArray[np.int_] | NDArray[np.bool_],
-                          state: list[int] = None):
+                          state: list[int] = None,
+                          mode: Literal['replace', 'append', 'exclude'] = 'replace'):
         """
         Capture electrodes.
 
         :param index: index (Array[E, N]) or bool (Array[bool, E]) array.
         :param state: restrict electrodes on given states.
+        :param mode:
         :see: {ProbeView#set_captured_electrodes()}
         """
         from .edit.probe import capture_electrode
         if (controller := self._controller) is not None:
-            capture_electrode(self, controller, index, state)
+            capture_electrode(self, controller, index, state, mode)
 
     @doc_link()
     def captured_electrodes(self, all=False) -> NDArray[np.int_]:
         """
         get captured electrodes.
 
         :param all: capture excluded electrodes?
@@ -1325,14 +1334,28 @@
         if (controller := self._controller) is not None:
             refresh_selection(self, controller, selector)
 
     # ====================== #
     # AtlasBrainView related #
     # ====================== #
 
+    @doc_link(Structure='neurocarto.util.atlas_struct.Structure')
+    def atlas_get_region_name(self, region: int | str) -> str | None:
+        """
+        Get region acronym.
+
+        :param region: region ID, acronym or its partial description
+        :return: region acronym
+        :see: {Structure}
+        """
+        from .edit.atlas import atlas_get_region_name
+        if (controller := self._controller) is not None:
+            return atlas_get_region_name(controller, region)
+        return None
+
     @doc_link()
     def atlas_get_slice(self, *, um=False) -> tuple[str | None, int | None]:
         """
         Get atlas brain image projection view and slicing plane.
 
         :param um: is plane index in return um? If so, then use bregma as origin.
         :return: tuple of (projection name, plane index)
@@ -1457,15 +1480,14 @@
         :param a: anchor point on image, center point as origin.
         :see: {BoundView#set_anchor_to()}
         """
         from .edit.atlas import atlas_set_anchor
         if (controller := self._controller) is not None:
             atlas_set_anchor(controller, p, a)
 
-    @doc_link()
     def atlas_new_probe(self,
                         ap: float, dv: float, ml: float,
                         shank: int = 0,
                         rx: float = 0, ry: float = 0, rz: float = 0,
                         depth: float = 0,
                         ref: str = 'bregma') -> ProbeCoordinate | None:
         """
@@ -1483,15 +1505,14 @@
         :return: a probe coordinate. ``None`` if origin not set.
         """
         from .edit.atlas import atlas_new_probe
         if (controller := self._controller) is not None:
             return atlas_new_probe(controller, ap, dv, ml, shank, rx, ry, rz, depth, ref)
         return None
 
-    @doc_link()
     def atlas_current_probe(self, shank: int = 0, ref: str = 'bregma') -> ProbeCoordinate | None:
         """
         Get the current coordinate of the probe.
 
         The dv value of the returned coordinate always zero.
 
         :param shank: which shank is the returned coordinate is based on.
@@ -1499,25 +1520,62 @@
         :return: a probe coordinate. ``None`` if origin not found.
         """
         from .edit.atlas import atlas_current_probe
         if (controller := self._controller) is not None:
             return atlas_current_probe(self, controller, shank, ref)
         return None
 
-    @doc_link()
     def atlas_set_anchor_on_probe(self, coor: ProbeCoordinate):
         """
         Update atlas image boundary transform to anchor insertion point onto the probe.
 
         :param coor: probe coordinate
         """
         from .edit.atlas import atlas_set_anchor_on_probe
         if (controller := self._controller) is not None:
             atlas_set_anchor_on_probe(self, controller, coor)
 
+    @doc_link()
+    def atlas_coor_electrode(self, coor: ProbeCoordinate = None,
+                             electrode: NDArray[np.int_] | NDArray[np.bool_] | NDArray[np.float_] = None,
+                             bregma: str | None = 'bregma') -> NDArray[np.float_]:
+        """
+        Transform electrode position to altas coordinate (AP,DV,ML) according the given probe coordinate.
+
+        :param coor: probe coordinate
+        :param electrode: electrode index (Array[int, N]), mask (Array[bool, E]) or position (Array[um:float, N, (x, y)])
+        :param bregma: use which bregma coordinate as origin.
+        :return: electrode position in Array[um:float, N, (ap, dv, ml)]
+        :see: use {#atlas_current_probe()} when *coor* is ``None``.
+        """
+        from .edit.atlas import atlas_coor_electrode
+        if (controller := self._controller) is None:
+            raise RuntimeError('cannot determine current atlas')
+
+        return atlas_coor_electrode(self, controller, coor, electrode, bregma)
+
+    @doc_link()
+    def atlas_mask_region(self, region: str, coor: ProbeCoordinate = None,
+                          electrode: NDArray[np.int_] | NDArray[np.bool_] | NDArray[np.float_] = None) -> NDArray[np.bool_]:
+        """
+        Return a mask that electrode located in the given region.
+
+        :param region: region name
+        :param coor: probe coordinate
+        :param electrode: electrode index (Array[int, N]), mask (Array[bool, E]) or position (Array[um:float, N, (x, y)])
+        :return: Array[bool, N]
+        :see: use {#atlas_current_probe()} when *coor* is ``None``.
+        :see: use {#atlas_coor_electrode()}
+        """
+        from .edit.atlas import atlas_mask_region
+        if (controller := self._controller) is None:
+            raise RuntimeError('cannot determine current atlas')
+
+        return atlas_mask_region(self, controller, region, coor, electrode)
+
     # =================== #
     # matplotlib plotting #
     # =================== #
 
     @doc_link(PltImageView='neurocarto.views.image_plt.PltImageView')
     def plot_channelmap(self, channelmap: M = None,
                         color: Any = 'black', *,
```

### Comparing `neurocarto-0.0.0/src/neurocarto/util/util_numpy.py` & `neurocarto-0.0.1/src/neurocarto/util/util_numpy.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/util/utils.py` & `neurocarto-0.0.1/src/neurocarto/util/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,17 @@
     attr = m.group('attr')
 
     try:
         value = sphinx_doc_link_get(context, attr)
     except KeyError:
         return m.group()
 
+    if not isinstance(value, str):
+        return m.group()
+
     if indent is None or len(indent) == 0:
         return value
 
     return textwrap.indent(value, indent)
 
 
 def sphinx_doc_link_replace_ref(context: list[dict], m: re.Match) -> str:
```

### Comparing `neurocarto-0.0.0/src/neurocarto/views/atlas.py` & `neurocarto-0.0.1/src/neurocarto/views/atlas.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,30 +585,30 @@
         c = [it.color for it in labels]
 
         boundary = self.get_boundary_state()
         a, a_ = probe_coor.prepare_affine_matrix_both(**boundary)
 
         origin = REFERENCE['bregma'][self.brain_view.brain.atlas_name]
 
-        qp = np.zeros_like(p)  # Array[float, 3, N]
-        qb = np.zeros((3, n), dtype=float)  # Array[float, 3, N]
+        qp = np.zeros_like(p)  # Array[um:float, 3, N]
+        qb = np.zeros((3, n), dtype=float)  # Array[mm:float, 3, N]
         for i, ref in enumerate(LABEL_REFS):
             if not np.any(mask := o == i):
                 continue
 
             match ref:
                 case 'probe':
                     q = p[:, mask]  # Array[float, (x,y,1), N']
                     qp[:, mask] = q
-                    qb[:, mask] = probe_coor.project_i2b(origin, self.brain_slice, (a_ @ q) / 1000)
+                    qb[:, mask] = probe_coor.project_i2b(origin, self.brain_slice, a_ @ q) / 1000
 
                 case 'image':
                     q = p[:, mask]  # Array[float, (x,y,1), N']
                     qp[:, mask] = a @ q
-                    qb[:, mask] = probe_coor.project_i2b(origin, self.brain_slice, q / 1000)
+                    qb[:, mask] = probe_coor.project_i2b(origin, self.brain_slice, q) / 1000
 
                 case 'bregma':
                     q = p[:, mask]  # Array[float, (ap,dv,ml), N']
                     qb[:, mask] = q
                     qp[:, mask] = a @ probe_coor.project_b2i(origin, self.brain_slice, q * 1000.0)
 
                 case str(bregma):
```

### Comparing `neurocarto-0.0.0/src/neurocarto/views/base.py` & `neurocarto-0.0.1/src/neurocarto/views/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,18 +568,18 @@
         pass
 
 
 class BoundaryState(TypedDict):
     """Boundary parameters"""
 
     dx: float
-    """x moving"""
+    """x moving (um)"""
 
     dy: float
-    """y moving"""
+    """y moving (um)"""
 
     sx: float
     """x scaling"""
 
     sy: float
     """y scaling"""
```

### Comparing `neurocarto-0.0.0/src/neurocarto/views/blueprint.py` & `neurocarto-0.0.1/src/neurocarto/views/blueprint.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/views/blueprint_script.py` & `neurocarto-0.0.1/src/neurocarto/views/blueprint_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         'move': 'neurocarto.util.edit._actions:move_blueprint',
         'exchange': 'neurocarto.util.edit._actions:exchange_shank',
         'single': 'neurocarto.util.edit._actions:npx24_single_shank',
         'stripe': 'neurocarto.util.edit._actions:npx24_stripe',
         'half': 'neurocarto.util.edit._actions:npx24_half_density',
         'quarter': 'neurocarto.util.edit._actions:npx24_quarter_density',
         '1-eighth': 'neurocarto.util.edit._actions:npx24_one_eighth_density',
+        'inside': 'neurocarto.util.edit._actions:highlight_electrode_inside_region',
         'optimize': 'neurocarto.util.edit._actions:optimize_channelmap',
         'label': 'neurocarto.util.edit._actions:atlas_label',
         'probe-coor': 'neurocarto.util.edit._actions:adjust_atlas_mouse_brain_to_probe_coordinate',
     }
     """Builtin scripts"""
 
     def __init__(self, config: CartoConfig):
```

### Comparing `neurocarto-0.0.0/src/neurocarto/views/data.py` & `neurocarto-0.0.1/src/neurocarto/views/data.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/views/data_density.py` & `neurocarto-0.0.1/src/neurocarto/views/data_density.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/views/image.py` & `neurocarto-0.0.1/src/neurocarto/views/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import abc
 import logging
 import sys
 from pathlib import Path
 from typing import TypedDict, Final
 
 import numpy as np
-from bokeh.models import ColumnDataSource, GlyphRenderer, Slider, UIElement, TextInput, Tooltip
+from bokeh.models import ColumnDataSource, GlyphRenderer, Slider, UIElement
 from numpy.typing import NDArray
 
 from neurocarto.config import CartoConfig
 from neurocarto.util.bokeh_app import run_later
-from neurocarto.util.bokeh_util import SliderFactory, is_recursive_called, PathAutocompleteInput, as_callback, new_help_button
+from neurocarto.util.bokeh_util import SliderFactory, is_recursive_called, PathAutocompleteInput, new_help_button
 from neurocarto.views.base import Figure, BoundView, StateView, BoundaryState
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
@@ -100,15 +100,17 @@
         from PIL import Image  # type: ignore[import]
         from .image_npy import NumpyImageHandler
 
         filename = str(filename)
         logger.debug('from file %s', filename)
         image = np.asarray(Image.open(filename, mode='r'))
 
-        w, h, _ = image.shape
+        w, h, c = image.shape
+        if c == 3:
+            image = np.dstack([image, np.full((w, h), 255, dtype=np.uint8)])
         image = np.flipud(image.view(dtype=np.uint32).reshape((w, h)))
 
         logger.debug('as image %s', image.shape)
         return NumpyImageHandler(image, filename)  # type: ignore[return-value]
 
     @classmethod
     def from_tiff(cls, filename: str | Path) -> Self:
@@ -183,18 +185,14 @@
             else:
                 slider.end = n_image
                 slider.disabled = False
 
             if self.visible:
                 slider.visible = not slider.disabled
 
-        if image is not None:
-            resolution = image.resolution
-            self.resolution_input.value = f'{resolution[0]},{resolution[1]}'
-
     def save_current_state(self) -> ImageViewState | None:
         if (image := self.image) is None:
             return None
 
         if (filename := image.filename) is None:
             return None
 
@@ -238,36 +236,22 @@
 
     def setup_image(self, f: Figure):
         self.render_image = f.image_rgba(
             'image', x='x', y='y', dw='dw', dh='dh', source=self.data_image,
             global_alpha=1, syncable=False,
         )
 
-    # TODO need a better design to provide resolution changing mechanism
-    # How do we distinguish an image source between resolution self-contained and not contained?
-    resolution_input: TextInput
-
-    def _setup_title(self, **kwargs) -> list[UIElement]:
-        ret = super()._setup_title(**kwargs)
-
-        self.resolution_input = TextInput(max_width=100, description=Tooltip(content='image resolution. format "10" or "10,10"'))
-        self.resolution_input.on_change('value', as_callback(self._on_resolution_changed))
-
-        # visible_btn?, view_title, help?, resolution_input, help, status_div
-        ret.insert(-1, self.resolution_input)
-        ret.insert(-1, new_help_button('change image resolution. Need a value or "W,H"', position='right'))
-
-        return ret
-
     index_slider: Slider = None
+    alpha_slider: Slider = None
 
     def _setup_content(self, slider_width: int = 300,
                        support_index=True,
                        support_rotate=True,
                        support_scale=True,
+                       support_alpha=False,
                        **kwargs) -> list[UIElement]:
         """
 
         :param slider_width:
         :param support_index: support image slide indexing.
         :param support_rotate: support image rotation
         :param support_scale: support image scaling
@@ -277,14 +261,16 @@
         from bokeh.layouts import row
 
         new_slider = SliderFactory(width=slider_width, align='end')
 
         ret = []
         if support_index:
             ret.append(row(*self.setup_index_slider(new_slider=new_slider)))
+        if support_alpha:
+            ret.append(row(*self.setup_alpha_slider(new_slider=new_slider)))
         if support_rotate:
             ret.append(row(*self.setup_rotate_slider(new_slider=new_slider)))
         if support_scale:
             ret.append(row(*self.setup_scale_slider(new_slider=new_slider)))
 
         return ret
 
@@ -294,63 +280,42 @@
             new_slider = SliderFactory(width=300, align='end')
 
         self.index_slider = new_slider('Index', (0, 1, 1, 0), self._on_index_changed)
         self.index_slider.visible = False
 
         return [self.index_slider]
 
+    def setup_alpha_slider(self, *,
+                           new_slider: SliderFactory = None) -> list[UIElement]:
+        if new_slider is None:
+            new_slider = SliderFactory(width=300, align='end')
+
+        self.alpha_slider = new_slider('Alpha', (0, 255, 1, 255), self._on_alpha_changed)
+
+        return [self.alpha_slider]
+
     def _on_index_changed(self, s: int):
         if is_recursive_called():
             return
 
         self.update_image(s)
 
-    def get_resolution_value(self, r: str = None) -> tuple[float, float] | None:
-        if r is None:
-            try:
-                r = self.resolution_input.value
-            except AttributeError:
-                return None
-
-        if r == '':
-            return None
-
-        try:
-            if ',' in r:
-                f = r.partition(',')
-                return float(f[0].strip()), float(f[2].strip())
-            else:
-                f = float(r)
-                return f, f
-        except ValueError:
-            return None
+    def _on_alpha_changed(self, a: int):
+        if is_recursive_called():
+            return
 
-    def _on_resolution_changed(self, r: str | float):
-        if is_recursive_called() or r == '':
+        if (image := self._image) is None:
             return
 
-        match r:
-            case str():
-                f = self.get_resolution_value(r)
-            case float(f):
-                f = (f, f)
-            case _:
-                raise TypeError()
-
-        if f is None:
-            if (image := self.image) is None:
-                self.resolution_input.value = ''
-            else:
-                f = image.resolution
-                self.resolution_input.value = f'{f[0]},{f[1]}'
+        try:
+            image.alpha = a
+        except AttributeError:
+            pass
         else:
-            if (image := self.image) is not None:
-                image.resolution = f
-
-            self.update_boundary_transform(s=1)
+            self.update_image(self.index_slider.value)
 
     # ================ #
     # updating methods #
     # ================ #
 
     def start(self):
         if self.image is not None:
@@ -473,17 +438,12 @@
 
         if state is None and image.filename is not None:
             try:
                 state = self.image_config[image.filename]
                 self.logger.debug('restore(%s)', image.filename)
             except KeyError:
                 self.logger.info('fail restore(%s) ', image.filename)
-                f = self.get_resolution_value()
-                if f is None:
-                    self.reset_boundary()
-                else:
-                    image.resolution = f
-                    self.update_boundary_transform(s=1)
+                self.reset_boundary()
                 return
 
         if state is not None:
             super().restore_current_state(state)
```

### Comparing `neurocarto-0.0.0/src/neurocarto/views/image_npy.py` & `neurocarto-0.0.1/src/neurocarto/views/image_npy.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,14 +36,36 @@
             return None
         elif image.ndim == 3:
             return image[index]
         else:
             return image
 
     @property
+    def alpha(self) -> int:
+        if (image := self.image) is None:
+            return 0
+
+        if image.ndim == 3:
+            image = image[0]
+
+        alpha = (image & 0xFF000000) >> 24
+
+        return int(np.unique(alpha)[0])
+
+    @alpha.setter
+    def alpha(self, value: int | float):
+        if (image := self.image) is None:
+            return
+
+        if isinstance(value, float):
+            value = int(255 * value)
+
+        self.image = (image & 0x00FFFFFF) | ((value << 24) & 0xFF000000)
+
+    @property
     def width(self) -> float:
         if (image := self.image) is None:
             return 0
 
         r = self.resolution[0]
         if image.ndim == 3:
             return image.shape[2] * r
```

### Comparing `neurocarto-0.0.0/src/neurocarto/views/image_plt.py` & `neurocarto-0.0.1/src/neurocarto/views/image_plt.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/views/probe.py` & `neurocarto-0.0.1/src/neurocarto/views/probe.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/views/record.py` & `neurocarto-0.0.1/src/neurocarto/views/record.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/views/utils.py` & `neurocarto-0.0.1/src/neurocarto/views/utils.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto/views/view_efficient.py` & `neurocarto-0.0.1/src/neurocarto/views/view_efficient.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/src/neurocarto.egg-info/PKG-INFO` & `neurocarto-0.0.1/src/neurocarto.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocarto
-Version: 0.0.0
+Version: 0.0.1
 Summary: A web-interface channelmap editor for Neuropixels probe familiy
 Author-email: Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, AntonioST
         
         Redistribution and use in source and binary forms, with or without
@@ -28,15 +28,15 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Homepage, https://github.com/AntonioST/NeuroCarto
-Project-URL: Documentation, https://github.com/AntonioST/NeuroCarto/wiki
+Project-URL: Documentation, https://neurocarto.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/AntonioST/NeuroCarto
 Project-URL: Issues, https://github.com/AntonioST/NeuroCarto/issues
 Keywords: Electrophysiology,Neuropixels,Channelmap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -57,14 +57,16 @@
 Requires-Dist: matplotlib
 Requires-Dist: typing_extensions
 Requires-Dist: bokeh
 
 NeuroCarto: A Neuropixels Channelmap Editor
 ===========================================
 
+[![PyPI - Version](https://img.shields.io/pypi/v/neurocarto)](https://pypi.org/project/neurocarto/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neurocarto)
 [![Documentation Status](https://readthedocs.org/projects/neurocarto/badge/?version=latest)](https://neurocarto.readthedocs.io/en/latest/?badge=latest)
 
 NeuroCarto is a neural probe channel map editor for the Neuropixels probe family.
 It allows user to create a blueprint for arranging electrodes in a desired density
 and generate a custom channel map.
 
 Features
@@ -92,16 +94,17 @@
 
 ### prepare environment.
 
 Require `Python 3.10`.
 
 ### Install
 
-
-This package will upload onto PyPI soon.
+```shell
+pip install neurocarto
+```
 
 ### Run
 
 ```shell
 neurocarto
 ```
```

### Comparing `neurocarto-0.0.0/src/neurocarto.egg-info/SOURCES.txt` & `neurocarto-0.0.1/src/neurocarto.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 src/neurocarto/util/edit/atlas.py
 src/neurocarto/util/edit/category.py
 src/neurocarto/util/edit/checking.py
 src/neurocarto/util/edit/clustering.py
 src/neurocarto/util/edit/data.py
 src/neurocarto/util/edit/debug.py
 src/neurocarto/util/edit/moving.py
+src/neurocarto/util/edit/optimize.py
 src/neurocarto/util/edit/plot.py
 src/neurocarto/util/edit/probe.py
 src/neurocarto/util/edit/script.py
 src/neurocarto/util/edit/surrounding.py
 src/neurocarto/views/__init__.py
 src/neurocarto/views/atlas.py
 src/neurocarto/views/base.py
```

### Comparing `neurocarto-0.0.0/tests/test_electrode_select.py` & `neurocarto-0.0.1/tests/test_electrode_select.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/tests/test_npx_probe.py` & `neurocarto-0.0.1/tests/test_npx_probe.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/tests/test_probe_oper.py` & `neurocarto-0.0.1/tests/test_probe_oper.py`

 * *Files identical despite different names*

### Comparing `neurocarto-0.0.0/tests/test_util_blueprint.py` & `neurocarto-0.0.1/tests/test_util_blueprint.py`

 * *Files identical despite different names*

