# Comparing `tmp/dataset_tools-0.0.85.tar.gz` & `tmp/dataset-tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_tools-0.0.85.tar", last modified: Wed May 22 13:59:12 2024, max compression
+gzip compressed data, was "dataset-tools-0.0.9.tar", last modified: Mon Jun  5 13:38:22 2023, max compression
```

## Comparing `dataset_tools-0.0.85.tar` & `dataset-tools-0.0.9.tar`

### file list

```diff
@@ -1,88 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.293412 dataset_tools-0.0.85/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-22 13:59:12.293412 dataset_tools-0.0.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.269412 dataset_tools-0.0.85/dataset_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.269412 dataset_tools-0.0.85/dataset_tools/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.273412 dataset_tools-0.0.85/dataset_tools/convert/cityscapes/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/convert/cityscapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/convert/cityscapes/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.273412 dataset_tools-0.0.85/dataset_tools/convert/coco/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/convert/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24946 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/convert/coco/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.273412 dataset_tools-0.0.85/dataset_tools/convert/pascal/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/convert/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19519 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/convert/pascal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.273412 dataset_tools-0.0.85/dataset_tools/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.273412 dataset_tools-0.0.85/dataset_tools/data/download_urls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/data/download_urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   229217 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/data/download_urls/released_datasets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.285412 dataset_tools-0.0.85/dataset_tools/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   491496 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   511708 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   473876 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   491048 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   481124 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   521088 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   431308 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   446916 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   456436 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   433824 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   447376 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   441384 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   456840 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   440984 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   473160 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   490704 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   426752 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   441292 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/fonts/FiraSans-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.285412 dataset_tools-0.0.85/dataset_tools/image/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.289412 dataset_tools-0.0.85/dataset_tools/image/renders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/horizontal_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    17874 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/poster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/previews.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/separated_anns_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/vertical_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/renders/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.289412 dataset_tools-0.0.85/dataset_tools/image/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/basestats.py
--rw-r--r--   0 runner    (1001) docker     (127)    20151 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/class_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    21119 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/class_cooccurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)    15793 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/classes_per_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/heatmaps_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23459 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/object_and_class_sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/objects_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/preview_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    30268 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/tags_cooccurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/image/stats/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.289412 dataset_tools-0.0.85/dataset_tools/repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/repo/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    41834 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/repo/project_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/repo/sample_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.289412 dataset_tools-0.0.85/dataset_tools/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/templates/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/templates/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/templates/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/templates/cv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/templates/licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.293412 dataset_tools-0.0.85/dataset_tools/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/dataset_tools/text/generate_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:12.293412 dataset_tools-0.0.85/dataset_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-22 13:59:12.000000 dataset_tools-0.0.85/dataset_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-22 13:59:12.000000 dataset_tools-0.0.85/dataset_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:59:12.000000 dataset_tools-0.0.85/dataset_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-22 13:59:12.000000 dataset_tools-0.0.85/dataset_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 13:59:12.000000 dataset_tools-0.0.85/dataset_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:59:12.293412 dataset_tools-0.0.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-22 13:56:32.000000 dataset_tools-0.0.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.023194 dataset-tools-0.0.9/dataset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/cityscapes/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/cityscapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/cityscapes/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/coco/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/convert/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/convert/pascal/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.031194 dataset-tools-0.0.9/dataset_tools/image/renders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/horizontal_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/poster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/separated_anns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/vertical_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/renders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.031194 dataset-tools-0.0.9/dataset_tools/image/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/basestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/class_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/class_cooccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/classes_per_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/heatmaps_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/object_and_class_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/objects_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/preview_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/image/stats/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.031194 dataset-tools-0.0.9/dataset_tools/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/dataset_tools/text/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/text/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/dataset_tools/text/summary/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:38:22.027194 dataset-tools-0.0.9/dataset_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 13:38:22.000000 dataset-tools-0.0.9/dataset_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:38:22.035194 dataset-tools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-05 13:35:37.000000 dataset-tools-0.0.9/setup.py
```

### Comparing `dataset_tools-0.0.85/LICENSE` & `dataset-tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset_tools-0.0.85/dataset_tools/convert/cityscapes/main.py` & `dataset-tools-0.0.9/dataset_tools/convert/cityscapes/main.py`

 * *Files identical despite different names*

### Comparing `dataset_tools-0.0.85/dataset_tools/convert/pascal/main.py` & `dataset-tools-0.0.9/dataset_tools/convert/pascal/main.py`

 * *Files identical despite different names*

### Comparing `dataset_tools-0.0.85/dataset_tools/image/renders/convert.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/convert.py`

 * *Files identical despite different names*

### Comparing `dataset_tools-0.0.85/dataset_tools/image/renders/horizontal_grid.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/horizontal_grid.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,75 @@
 import os
 import random
 from typing import Union
 
 import cv2
 import numpy as np
-import supervisely as sly
-from supervisely.imaging import font as sly_font
 from tqdm import tqdm
 
-from dataset_tools.image.renders.convert import (
-    compress_mp4,
-    compress_png,
-    from_mp4_to_webm,
-)
+import supervisely as sly
+from dataset_tools.image.renders.convert import from_mp4_to_webm, compress_mp4, compress_png
 
 
 class HorizontalGrid:
     def __init__(
         self,
         project: Union[str, int],
         project_meta: sly.ProjectMeta,
         api: sly.Api = None,
         rows: int = 3,
-        cols: int = 4,
+        cols: int = 6,
         force: bool = False,
-        is_detection_task: bool = False,
     ):
         self.force = force
         self.project_meta = project_meta
-        self._is_detection_task = is_detection_task
 
+        self._img_height = 1920
         self._rows = rows
         self._cols = cols
         self._gap = 15
         self._row_width = 0
-        default_img_height = 1920
-        row_height = int((default_img_height - self._gap * (self._rows + 1)) / self._rows)
-        self._row_height = row_height if row_height < 500 else 500
-        self._img_height = self._row_height * self._rows + self._gap * (self._rows + 1)
-
         self._logo_path = "logo.png"
-        self.fps = 15
-        self.duration = 2
-        self.pause = 5
-        self.num_frames = int(self.duration * self.fps)
 
         self.np_images = []  # for grid
-        self.np_frames = {i: [] for i in range(self.num_frames + self.pause)}  # for gif
+        self.np_anns = []  # for gif
+        self.np_frames = []  # for gif
         self._img_array = None
+        self._row_height = int((self._img_height - self._gap * (self._rows + 1)) / self._rows)
 
         self._local = False if isinstance(project, int) else True
         self._api = api if api is not None else sly.Api.from_env()
 
     @property
     def basename_stem(self) -> None:
         return sly.utils.camel_to_snake(self.__class__.__name__)
 
     def update(self, data: tuple):
         cnt = self._cols * self._rows
-        # data = [data[1]]  # hack to get pull of images only from specific ds
         join_data = [(ds, img, ann) for ds, list1, list2 in data for img, ann in zip(list1, list2)]
 
         random.shuffle(join_data)
-        with tqdm(desc="HorizontalGrid: downloading images", total=cnt) as p:
-            i = 0
-            while len(self.np_images) < cnt:
-                ds, img_info, ann = join_data[i]
+        with tqdm(desc="Downloading images", total=cnt) as p:
+            for ds, img_info, ann in join_data[:cnt]:
                 img = (
                     sly.image.read(ds.get_img_path(img_info.name))
                     if self._local
                     else self._api.image.download_np(img_info.id)
                 )
+                p.update(1)
                 ann: sly.Annotation
-                img = self._resize_image(img, self._row_height)
-                try:
-                    def _resize_label(label):
-                        try:
-                            return [label.resize(ann.img_size, img.shape[:2])]
-                        except:
-                            return []
-
-                    ann = ann.transform_labels(_resize_label, img.shape[:2])
-                except Exception:
-                    sly.logger.warn(
-                        f"Skipping image: can not resize annotation. Image name: {img_info.name}"
-                    )
-                    continue
-                self.np_images.append(self._draw_annotation(ann, img))
-
-                tmp = np.dstack((np.copy(img), np.ones((*img.shape[:2], 1), dtype=np.uint8) * 255))
-                for j in list(range(0, len(self.np_frames))):
-                    alpha = j / self.num_frames
-                    if j >= self.num_frames:
-                        alpha = round(1 - random.uniform(0, 0.03), 3)
-                    frame = self._draw_annotation(ann, tmp, alpha)
-                    self.np_frames[j].append(frame)
+                tmp = np.dstack((img, np.ones((*img.shape[:2], 1), dtype=np.uint8) * 255))
+                ann_mask = np.ones((*img.shape[:2], 4), dtype=np.uint8) * 255
+                ann.draw_pretty(ann_mask[:, :, :3], thickness=0, opacity=0.7)
+                self.np_frames.append(self._resize_image(tmp, self._row_height))  # for gif
+                self.np_anns.append(self._resize_image(ann_mask, self._row_height))  # for gif
 
-                i += 1
-                p.update(1)
+                ann.draw_pretty(img, thickness=0, opacity=0.7)  # for grid
+                img = self._resize_image(img, self._row_height)
+                self.np_images.append(img)
 
     def to_image(self, path: str = None):
         path_part, ext = os.path.splitext(path)
         tmp_path = f"{path_part}-o{ext}"
         if path is None:
             storage_dir = sly.app.get_data_dir()
             path = os.path.join(storage_dir, "horizontal_grid.png")
@@ -111,31 +79,36 @@
 
         sly.image.write(tmp_path, self._img_array)
         compress_png(tmp_path, path)
         sly.fs.silent_remove(tmp_path)
         sly.logger.info(f"Result grid saved to: {path}")
 
     def animate(self, path: str = None):
+        bg = self._merge_canvas_with_images(self.np_frames, 4)
+        ann = self._merge_canvas_with_images(self.np_anns, 4)
+        ann[:, :, 3] = np.where(np.all(ann == 255, axis=-1), 0, 255).astype(np.uint8)
+
+        duration = 1.1
+        fps = 15
+        num_frames = int(duration * fps)
         frames = []
-        n = [*range(0, self.num_frames + self.pause), *range(self.num_frames, 0, -1)]
-        with tqdm(desc="HorizontalGrid: prepare frames...", total=len(n)) as vid_pbar:
-            for i in n:
-                frame = self._merge_canvas_with_images(self.np_frames[i])
-                self._add_logo(frame)
-                frame = self._resize_image(frame, frame.shape[0] // 2)
-                frame = cv2.cvtColor(frame, cv2.COLOR_RGB2BGR)
-                frames.append(frame)
-                vid_pbar.update(1)
+        for i in list(range(1, num_frames + 1)) + list(range(num_frames, 0, -1)):
+            alpha = i / num_frames
+            frame = self._overlay_images(bg, ann, alpha)
+            self._add_logo(frame)
+            frame = self._resize_image(frame, frame.shape[0] // 2)
+            frames.append(frame)
+            if i == num_frames:
+                frames.extend([frame] * (fps // 2))
 
         tmp_video_path = f"{os.path.splitext(path)[0]}-o.mp4"
         video_path = f"{os.path.splitext(path)[0]}.mp4"
         self._save_video(tmp_video_path, frames)
-        sly.logger.info("Compression and conversion to webm...")
+        from_mp4_to_webm(tmp_video_path, path)
         compress_mp4(tmp_video_path, video_path)
-        from_mp4_to_webm(video_path, path)
         sly.fs.silent_remove(tmp_video_path)
 
         sly.logger.info(f"Animation saved to: {path}, {video_path}")
 
     def _merge_canvas_with_images(self, images, channels: int = 3):
         rows = self._create_rows(images)
         rows = self._merge_img_in_rows(rows, channels)
@@ -155,33 +128,28 @@
             canvas[row_start:row_end, column_start:column_end] = image
         return canvas
 
     def _create_rows(self, images):
         num_images = len(images)
         image_widths = [image.shape[1] for image in images]
 
-        one_big_row_width = sum(image_widths) + (num_images - 1) * self._gap
+        one_big_row_width = sum(image_widths[: -self._rows]) + (num_images - 1) * self._gap
         self._row_width = one_big_row_width // self._rows
 
         rows = []
         row_images = []
         current_width = 0
 
         for idx, (image, width) in enumerate(zip(images, image_widths)):
-            if current_width + width > self._row_width:
+            if current_width + width > self._row_width or idx == len(images) - 1:
                 rows.append(row_images)
 
                 row_images = []
                 current_width = 0
-                if len(rows) == self._rows:
-                    return rows
             row_images.append(image)
-            if idx == len(images) - 1:
-                rows.append(row_images)
-                return rows
             current_width += width + self._gap
 
         return rows
 
     def _merge_img_in_rows(self, rows, channels: int = 3):
         max_width = 0
         img_widths = []
@@ -245,46 +213,15 @@
         return result_image
 
     def _save_video(self, videopath: str, frames):
         fourcc = cv2.VideoWriter_fourcc(*"VP90")
         height, width = frames[0].shape[:2]
         video_writer = cv2.VideoWriter(videopath, fourcc, 15, (width, height))
 
-        with tqdm(desc="HorizontalGrid: Saving video...", total=len(frames)) as vid_pbar:
+        with tqdm(desc="Saving video...", total=len(frames)) as vid_pbar:
             for frame in frames:
+                if frame.shape[:2] != (height, width):
+                    raise Exception("Not all frame sizes are not equal to each other.")
+                frame = cv2.cvtColor(frame, cv2.COLOR_RGBA2BGR)
                 video_writer.write(frame)
                 vid_pbar.update(1)
         video_writer.release()
-
-    def _draw_annotation(self, ann: sly.Annotation, img: np.ndarray, opacity: float = 0.7):
-        result = np.copy(img[:, :, :3])
-        thickness = ann._get_thickness()
-        font_size = int(sly_font.get_readable_font_size(result.shape[:2]) * 1.4)
-        font = sly_font.get_font(font_size=font_size)
-
-        rect_labels = [label for label in ann.labels if type(label.geometry) == sly.Rectangle]
-        other_labels = [label for label in ann.labels if type(label.geometry) != sly.Rectangle]
-        ann_without_rects = ann.clone(labels=other_labels)
-
-        if not self._is_detection_task:
-            ann_without_rects.draw_pretty(
-                result, thickness=0, opacity=opacity, fill_rectangles=False
-            )
-        if len(rect_labels) > 0:
-            ann_rects = ann.clone(labels=rect_labels)
-            ann_mask = np.ones((*img.shape[:2], 3), dtype=np.uint8) * 255
-            for label in ann_rects.labels:
-                label.draw_contour(ann_mask, thickness=thickness)
-                if self._is_detection_task:
-                    bbox = label.geometry.to_bbox()
-                    pt1, pt2 = (bbox.left, bbox.top), (bbox.right, bbox.bottom)
-                    cv2.rectangle(ann_mask, pt1, pt2, label.obj_class.color, thickness=thickness)
-                    _, _, _, bottom = font.getbbox(label.obj_class.name)
-                    anchor = (bbox.top - bottom, bbox.left)
-                    sly.image.draw_text(
-                        ann_mask, label.obj_class.name, anchor, font=font, fill_background=True
-                    )
-            ann_mask = np.dstack((ann_mask, np.ones((*img.shape[:2], 1), dtype=np.uint8) * 255))
-            ann_mask[:, :, 3] = np.where(np.all(ann_mask == 255, axis=-1), 0, 255).astype(np.uint8)
-
-            result = self._overlay_images(result, ann_mask, opacity=opacity)
-        return result
```

### Comparing `dataset_tools-0.0.85/dataset_tools/image/renders/separated_anns_grid.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/vertical_grid.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,222 +3,226 @@
 from typing import Union
 
 import cv2
 import numpy as np
 from tqdm import tqdm
 
 import supervisely as sly
-from supervisely.imaging import font as sly_font
-from dataset_tools.image.renders.convert import compress_png
+from dataset_tools.image.renders.convert import from_mp4_to_webm, compress_mp4, compress_png
 
 
-class SideAnnotationsGrid:
+class VerticalGrid:
     def __init__(
         self,
         project: Union[str, int],
         project_meta: sly.ProjectMeta,
         api: sly.Api = None,
-        rows: int = 2,
-        cols: int = 4,
+        rows: int = 6,
+        cols: int = 3,
+        footer_path: str = "dninja_footer.png",
         force: bool = False,
-        is_detection_task: bool = False,
     ):
         self.force = force
         self.project_meta = project_meta
-        self._is_detection_task = is_detection_task
 
-        self._img_height = 1080
+        self._img_width = 1920
         self._rows = rows
         self._cols = cols
-        self._row_width = 0
-        self._gap = 15
-        self._bg_color = (221, 210, 230)  # rgb(221, 210, 230)
+        self._g_spacing = 15
+        self._column_height = 0
+        self._footer_path = footer_path
+
+        self.np_images = []  # for grid
+        self.np_anns = []  # for gif
+        self.np_frames = []  # for gif
+        self._img_array = None
+        self._column_width = int(
+            (self._img_width - self._g_spacing * (self._cols + 1)) / self._cols
+        )
 
         self._local = False if isinstance(project, int) else True
         self._api = api if api is not None else sly.Api.from_env()
 
-        self.np_images = []
-        self._img_array = None
-        self._row_height = int((self._img_height - self._gap * (self._rows + 1)) / self._rows)
-
-        self._side_overlay_path = "side_logo_overlay.png"
-        self._logo_path = "logo.png"
-
     @property
     def basename_stem(self) -> None:
         return sly.utils.camel_to_snake(self.__class__.__name__)
 
     def update(self, data: tuple):
         cnt = self._cols * self._rows
         join_data = [(ds, img, ann) for ds, list1, list2 in data for img, ann in zip(list1, list2)]
 
         random.shuffle(join_data)
-        with tqdm(desc="SideAnnotationsGrid: download images", total=cnt) as p:
+        with tqdm(desc="Downloading images", total=cnt) as p:
             for ds, img_info, ann in join_data[:cnt]:
+                ann: sly.Annotation
                 img = (
                     sly.image.read(ds.get_img_path(img_info.name))
                     if self._local
                     else self._api.image.download_np(img_info.id)
                 )
-                mask = self._draw_masks_on_single_image(ann, img_info)
-
-                img = self._resize_image(img)
-                mask = self._resize_image(mask)
-                join_image = np.hstack([img, mask])
-                self.np_images.append(join_image)
+                tmp = np.dstack((img, np.ones((*img.shape[:2], 1), dtype=np.uint8) * 255))
+                ann_mask = np.ones((*img.shape[:2], 4), dtype=np.uint8) * 255
+                ann.draw_pretty(ann_mask[:, :, :3], thickness=0, opacity=0.7)
+                self.np_frames.append(self._resize_image(tmp, self._column_width))  # for gif
+                self.np_anns.append(self._resize_image(ann_mask, self._column_width))  # for gif
+
+                ann.draw_pretty(img, thickness=0, opacity=0.7)
+                img = self._resize_image(img, self._column_width)
+                self.np_images.append(img)
 
                 p.update(1)
 
-    def _draw_masks_on_single_image(self, ann: sly.Annotation, image: sly.ImageInfo):
-        height, width = image.height, image.width
-        mask_img = np.zeros((height, width, 3), dtype=np.uint8)
-        mask_img[:, :, 0:3] = self._bg_color  # rgb(221, 210, 230)
-
-        for label in ann.labels:
-            if type(label.geometry) == sly.Point:
-                label.draw(mask_img, thickness=15)
-            elif self._is_detection_task:
-                bbox = label.geometry.to_bbox()
-                pt1, pt2 = (bbox.left, bbox.top), (bbox.right, bbox.bottom)
-                thickness = ann._get_thickness()
-                cv2.rectangle(mask_img, pt1, pt2, label.obj_class.color, thickness)
-                font_size = int(sly_font.get_readable_font_size(mask_img.shape[:2]) * 1.4)
-                font = sly_font.get_font(font_size=font_size)
-                _, _, _, bottom = font.getbbox(label.obj_class.name)
-                anchor = (bbox.top - bottom, bbox.left)
-                sly.image.draw_text(mask_img, label.obj_class.name, anchor, font=font)
-        if not self._is_detection_task:
-            ann.draw_pretty(mask_img, thickness=3, opacity=0.7, fill_rectangles=False)
-
-        return mask_img
-
     def to_image(self, path: str = None):
         path_part, ext = os.path.splitext(path)
         tmp_path = f"{path_part}-o{ext}"
         if path is None:
             storage_dir = sly.app.get_data_dir()
-            path = os.path.join(storage_dir, "horizontal_grid.png")
-
-        self._merge_canvas_with_images()
-        self._add_logo(self._img_array)
+            path = os.path.join(storage_dir, "vertical_grid.png")
+        self._img_array = self._merge_canvas_with_images(self.np_images)
+        self._add_footer_with_logo(self._img_array)
 
         sly.image.write(tmp_path, self._img_array)
-        compress_png(tmp_path, path)
+        compress_png(tmp_path, path, 1080)
         sly.fs.silent_remove(tmp_path)
         sly.logger.info(f"Result grid saved to: {path}")
 
-    def _create_image_canvas(self):
-        self._img_array = np.ones([self._img_height, self._row_width, 3], dtype=np.uint8) * 255
-
-    def _merge_canvas_with_images(self):
-        rows = self._create_rows()
-        rows = self._merge_img_in_rows(rows)
-        self._create_image_canvas()
-        for i, image in enumerate(rows):
-            if i >= self._rows:
-                continue
-            if image.shape[1] > self._img_array.shape[1] - self._gap:
-                image = image[:, : self._img_array.shape[1] - self._gap]
-
-            row_start = i * (self._row_height + self._gap) + self._gap
-            row_end = row_start + self._row_height
-            column_start = self._gap
-            column_end = self._img_array.shape[1]
-
-            self._img_array[row_start:row_end, column_start:column_end] = image
-        self._img_array[:, -self._gap :] = 255
-
-    def _create_rows(self):
-        num_images = len(self.np_images)
-        image_widths = [image.shape[1] for image in self.np_images]
-
-        one_big_row_width = sum(image_widths) + (num_images - 1) * self._gap
-        self._row_width = one_big_row_width // self._rows
-
-        rows = []
-        row_images = []
-        current_width = 0
-
-        for idx, (image, width) in enumerate(zip(self.np_images, image_widths)):
-            if current_width + width > self._row_width:
-                rows.append(row_images)
-                if len(rows) == self._rows:
-                    return rows
-
-                row_images = []
-                current_width = 0
-
-            row_images.append(image)
-            if idx == num_images - 1:
-                rows.append(row_images)
-                return rows
-            current_width += width + self._gap
-
-        return rows
-
-    def _merge_img_in_rows(self, rows):
-        combined_rows = []
-        separator = np.ones((self._row_height, 15, 3), dtype=np.uint8) * 255
-        for row in rows:
+    def animate(self, path: str = None):
+        bg = self._merge_canvas_with_images(self.np_frames, 4)
+        ann = self._merge_canvas_with_images(self.np_anns, 4)
+        ann[:, :, 3] = np.where(np.all(ann == 255, axis=-1), 0, 255).astype(np.uint8)
+
+        duration = 1.1
+        fps = 15
+        num_frames = int(duration * fps)
+        frames = []
+        for i in list(range(1, num_frames + 1)) + list(range(num_frames, 0, -1)):
+            alpha = i / num_frames
+            frame = self._overlay_images(bg, ann, alpha)
+            self._add_footer_with_logo(frame)
+            frame = self._resize_image(frame, frame.shape[1] // 2)
+            frames.append(frame)
+            if i == num_frames:
+                frames.extend([frame] * (fps // 2))
+
+        tmp_video_path = f"{os.path.splitext(path)[0]}-o.mp4"
+        video_path = f"{os.path.splitext(path)[0]}.mp4"
+        self._save_video(tmp_video_path, frames)
+        from_mp4_to_webm(tmp_video_path, path)
+        compress_mp4(tmp_video_path, video_path)
+        sly.fs.silent_remove(tmp_video_path)
+
+        sly.logger.info(f"Animation saved to: {path}, {video_path}")
+
+    def _merge_canvas_with_images(self, images, channels: int = 3):
+        columns = self._create_columns(images)
+        columns = self._merge_img_in_columns(columns, channels)
+
+        canvas = np.ones([self._column_height, self._img_width, channels], dtype=np.uint8) * 255
+        for i, image in enumerate(columns):
+            if image.shape[0] > canvas.shape[0] - self._g_spacing:
+                image = image[: canvas.shape[0] - self._g_spacing, :]
+
+            column_start = i * (self._column_width + self._g_spacing) + self._g_spacing
+            column_end = column_start + self._column_width
+            row_start = self._g_spacing
+            row_end = canvas.shape[0]
+
+            canvas[row_start:row_end, column_start:column_end] = image
+
+        return canvas
+
+    def _create_columns(self, images):
+        num_images = len(images)
+        image_heights = [image.shape[0] for image in images]
+
+        one_big_column_height = (
+            sum(image_heights[: -self._cols]) + (num_images - 2) * self._g_spacing
+        )
+        self._column_height = one_big_column_height // self._cols
+
+        columns = []
+        column_images = []
+        current_height = 0
+
+        for image, height in zip(images, image_heights):
+            column_images.append(image)
+            current_height += height + self._g_spacing
+
+            if current_height > self._column_height:
+                columns.append(column_images)
+
+                column_images = []
+                current_height = 0
+
+        if len(columns) == self._cols:
+            return columns
+        return columns
+
+    def _merge_img_in_columns(self, columns, channels: int = 3):
+        combined_columns = []
+        separator = np.ones((15, self._column_width, channels), dtype=np.uint8) * 255
+        for column in columns:
             combined_images = []
 
-            for image in row:
+            for image in column:
                 combined_images.append(image)
                 combined_images.append(separator)
             combined_images.pop()
-            combined_image = np.hstack(combined_images)
-            combined_rows.append(combined_image)
+            combined_image = np.vstack(combined_images)
+            combined_columns.append(combined_image)
 
-        self._row_width = min([img.shape[1] for img in combined_rows])
-        return combined_rows
+        return combined_columns
 
-    def _resize_image(self, image, height=None):
+    def _resize_image(self, image, width):
         img_h, img_w = image.shape[:2]
-        if height is None:
-            height = self._row_height
-        img_aspect_ratio = height / img_h
-        img_h = int(height)
-        img_w = int(img_aspect_ratio * img_w)
+        img_aspect_ratio = width / img_w
+        img_w = int(width)
+        img_h = int(img_aspect_ratio * img_h)
 
         image = sly.image.resize(image, (img_h, img_w))
 
         return image
 
-    def _add_overlay_with_logo(self):
-        image2 = cv2.imread(self._side_overlay_path, cv2.IMREAD_UNCHANGED)
+    def _add_footer_with_logo(self, image):
+        image2 = cv2.imread(self._footer_path, cv2.IMREAD_UNCHANGED)
         image2 = cv2.cvtColor(image2, cv2.COLOR_BGRA2RGBA)
 
-        _, width1 = self._img_array.shape[:2]
+        height1, width1 = image.shape[:2]
         height2, width2 = image2.shape[:2]
 
-        alpha_channel = image2[:, :, 3] / 255.0
-
-        x = width1 - width2
+        if width1 != width2:
+            scale_factor = width1 / width2
+            height2, width2 = int(scale_factor * height2), width1
+            image2 = sly.image.resize(image2, (height2, width2))
 
-        region = self._img_array[:height2, x : x + width2]
-        self._img_array[:height2, x : x + width2, :3] = (
-            1 - alpha_channel[:, :, np.newaxis]
-        ) * region + alpha_channel[:, :, np.newaxis] * image2[:, :, :3]
-
-    def _add_logo(self, image):
-        height = max(self._row_height // 5, 80)
-        image2 = cv2.imread(self._logo_path, cv2.IMREAD_UNCHANGED)
-        image2 = cv2.cvtColor(image2, cv2.COLOR_BGRA2RGBA)
-        image2 = self._resize_image(image2, height)
+        alpha_channel = image2[:, :, 3] / 255.0
 
-        height_r = height
-        while image2.shape[1] > image.shape[1] * 0.25:
-            height_r = int(0.95 * height_r)
-            image2 = self._resize_image(image2, height_r)
-
-        h1, w1 = image.shape[:2]
-        h2, w2 = image2.shape[:2]
-        x = w1 - w2 - self._gap * 2
-        y = h1 - h2 - self._gap * 2
-        alpha = image2[:, :, 3] / 255.0
-
-        reg = image[y : y + h2, x : x + w2]
-        image[y : y + h2, x : x + w2, :3] = (1 - alpha[:, :, np.newaxis]) * reg[:, :, :3] + alpha[
-            :, :, np.newaxis
-        ] * image2[:, :, :3]
+        x = 0
+        y = height1 - height2
 
-        return image
+        region = image[y:height1, x : x + width2]
+        image[y:height1, x : x + width2, :3] = (1 - alpha_channel[:, :, np.newaxis]) * region[
+            :, :, :3
+        ] + alpha_channel[:, :, np.newaxis] * image2[:, :, :3]
+
+    def _overlay_images(self, bg, overlay, opacity):
+        alpha = overlay[..., 3] * opacity / 255.0
+        one_minus_alpha = 1 - alpha
+
+        result_image = np.copy(bg)
+        for c in range(3):
+            result_image[..., c] = bg[..., c] * one_minus_alpha + overlay[..., c] * alpha
+        return result_image
+
+    def _save_video(self, videopath: str, frames):
+        fourcc = cv2.VideoWriter_fourcc(*"VP90")
+        height, width = frames[0].shape[:2]
+        video_writer = cv2.VideoWriter(videopath, fourcc, 15, (width, height))
+
+        with tqdm(desc="Saving video...", total=len(frames)) as vid_pbar:
+            for frame in frames:
+                if frame.shape[:2] != (height, width):
+                    raise Exception("Not all frame sizes are not equal to each other.")
+                frame = cv2.cvtColor(frame, cv2.COLOR_RGBA2BGR)
+                video_writer.write(frame)
+                vid_pbar.update(1)
+        video_writer.release()
```

### Comparing `dataset_tools-0.0.85/dataset_tools/image/renders/wrapper.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,84 +9,57 @@
     api: sly.Api,
     project: Union[int, str],
     datasets: List[Union[sly.DatasetInfo, sly.Project.DatasetDict]],
     meta: sly.ProjectMeta,
     sample_cnt: float,
 ):
     total = 0
-    classification_only = False
     samples = []
-    datasets_with_labels = []
-
     for dataset in datasets:
+        dataset: sly.Dataset
+        k = min(
+            sample_cnt // len(datasets),
+            (dataset.items_count if isinstance(project, int) else len(os.listdir(dataset.ann_dir))),
+        )
+
         ds_images = (
             api.image.get_list(
                 dataset.id,
                 filters=[{"field": "labelsCount", "operator": ">", "value": 0}],
             )
             if isinstance(project, int)
             else [
                 dataset.get_image_info(sly.fs.get_file_name(img))
                 for img in os.listdir(dataset.ann_dir)
                 if dataset.get_image_info(sly.fs.get_file_name(img)).labels_count > 0
             ]
         )
-        if len(ds_images) < sample_cnt // len(datasets):
-            continue
-        datasets_with_labels.append((dataset, ds_images))
-
-    if len(datasets_with_labels) == 0:
-        datasets_without_labels = []
-        for dataset in datasets:
-            ds_images = (
-                api.image.get_list(dataset.id)
-                if isinstance(project, int)
-                else [
-                    dataset.get_image_info(sly.fs.get_file_name(img))
-                    for img in os.listdir(dataset.ann_dir)
-                ]
-            )
-            datasets_without_labels.append((dataset, ds_images))
-
-        datasets_with_labels = datasets_without_labels  # classification-only case
-        classification_only = True
-
-    for dataset, ds_images in datasets_with_labels:
-        dataset: sly.Dataset
-        k = min(
-            sample_cnt // len(datasets_with_labels),
-            (dataset.items_count if isinstance(project, int) else len(os.listdir(dataset.ann_dir))),
-        )
 
         s = random.sample(ds_images, min(k, len(ds_images)))
         anns = (
             [
                 sly.Annotation.from_json(ann_json, meta)
                 for ann_json in api.annotation.download_json_batch(
                     dataset.id,
                     [item.id for item in s],
                 )
             ]
             if isinstance(project, int)
             else [dataset.get_ann(img.name, meta) for img in s]
         )
         samples.append((dataset, s, anns))
-        total += len(s)
-
-    total = -1 if classification_only else total
+        total += k
     return samples, total
 
 
 def prepare_renders(
     project: Union[int, str], renderers: list, sample_cnt: int = 25, api: sly.Api = None
 ) -> None:
     if len(renderers) == 0:
-        print(
-            "Passed 'renderers' parameter is empty. Enable 'force' flag to overwrite renderers output file. Skipping renderers preparation..."
-        )
+        print("Passed 'renderers' parameter is empty. Enable 'force' flag to overwrite renderers output file. Skipping renderers preparation...")
         return
     if api is None:
         api = sly.Api.from_env()
     if isinstance(project, int):
         project_meta = sly.ProjectMeta.from_json(api.project.get_meta(project))
         datasets = api.dataset.get_list(project)
     elif isinstance(project, str):
@@ -96,13 +69,9 @@
     else:
         raise ValueError("Project should be either an integer project ID or a string project path.")
 
     samples, total = sample_images(api, project, datasets, project_meta, sample_cnt)
     if len(samples) == 0:
         raise Exception("There are not any images with labels on them in the project.")
 
-    if total == -1:
-        poster = renderers[0]
-        poster.update_unlabeled(samples)
-    else:
-        for renderer in renderers:
-            renderer.update(samples)
+    for renderer in renderers:
+        renderer.update(samples)
```

### Comparing `dataset_tools-0.0.85/dataset_tools/repo/sample_project.py` & `dataset-tools-0.0.9/dataset_tools/image/renders/separated_anns_grid.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,185 +1,175 @@
-from __future__ import annotations
-
+import os
 import random
-from typing import Callable, Dict, Generator, List, NamedTuple, Optional, Tuple, Union
+from typing import Union
+
+import cv2
+import numpy as np
+from tqdm import tqdm
 
 import supervisely as sly
-from supervisely import OpenMode, Project
-from supervisely._utils import batched, is_development
-from supervisely.annotation.annotation import Annotation, TagCollection
-from supervisely.project.project_meta import ProjectMeta
-from supervisely.task.progress import Progress
-
-
-def get_sample_image_infos(
-    api,
-    project_info: sly.ProjectInfo,
-    project_stats: dict,
-    class_balance_json: dict = None,
-    is_classification_cvtask=False,
-) -> List[sly.ImageInfo]:
-    MAX_WEIGHT_BYTES = 5e8
-    MAX_ITEMS_COUNT = 1e3
-
-    mean_size = int(project_info.size) / project_info.items_count
-    MIN_ITEMS_COUNT_PER_CLASS = 5 if mean_size > 1e6 else 10
-    total_num_classes = len(project_stats["images"]["objectClasses"])
-    MIN_ITEMS_COUNT_PER_CLASS = (
-        1 if mean_size > 1e6 and total_num_classes > 40 else MIN_ITEMS_COUNT_PER_CLASS
-    )
-
-    if (
-        int(project_info.size) < MAX_WEIGHT_BYTES
-        and int(project_info.items_count) < MAX_ITEMS_COUNT
-    ) or int(project_info.size) < 7e8:
-        return None
-
-    datasets = api.dataset.get_list(project_info.id)
-
-    optimal_size = min(MAX_ITEMS_COUNT * mean_size, MAX_WEIGHT_BYTES)
-    optimal_items_count = int(optimal_size / mean_size)
-
-    if class_balance_json is None or total_num_classes > 1000 or is_classification_cvtask:
-        full_list = []
-        for dataset in datasets:
-            full_list += api.image.get_list(dataset.id)
-        return_count = (
-            optimal_items_count if len(full_list) > optimal_items_count else len(full_list)
-        )
-        return random.sample(full_list, return_count)
-
-    classes_on_marked_images_sum = sum(row[1] for row in class_balance_json["data"])
-    images_marked_sum = project_stats["images"]["total"]["imagesMarked"]
-    images_not_marked_sum = project_stats["images"]["total"]["imagesNotMarked"]
-
-    value_factor = (
-        images_marked_sum / images_not_marked_sum
-        if images_not_marked_sum > images_marked_sum
-        else 1
-    )
-
-    classes_per_image = classes_on_marked_images_sum / images_marked_sum
-
-    classes_on_all_images_sum = (
-        classes_on_marked_images_sum + images_not_marked_sum * classes_per_image
-    )
-    sample_factor = optimal_items_count / classes_on_all_images_sum
-
-    demo_data = []
-    for class_row, img_references in zip(
-        class_balance_json["data"],
-        class_balance_json["referencesRow"],
+from dataset_tools.image.renders.convert import compress_png
+
+
+class SideAnnotationsGrid:
+    def __init__(
+        self,
+        project: Union[str, int],
+        project_meta: sly.ProjectMeta,
+        api: sly.Api = None,
+        rows: int = 3,
+        cols: int = 3,
+        side_overlay_path: str = "side_logo_overlay.png",
+        force: bool = False,
     ):
-        class_items_count = class_row[1]
-        sampled_items_count = max(MIN_ITEMS_COUNT_PER_CLASS, int(class_items_count * sample_factor))
+        self.force = force
+        self.project_meta = project_meta
 
-        if len(img_references) > sampled_items_count:
-            indices = sorted(random.sample(range(len(img_references)), sampled_items_count))
-            demo_data += [img_references[i] for i in indices]
-        else:
-            demo_data += img_references
-
-    shrinkage_factor = len(set(demo_data)) / len(demo_data)
-    demo_data = list(set(demo_data))
-
-    imagesNotMarked_by_ds = {
-        ds["id"]: int(
-            ds["imagesNotMarked"]
-            * sample_factor
-            * classes_per_image
-            * shrinkage_factor
-            * value_factor
-        )
-        for ds in project_stats["images"]["datasets"]
-    }
-
-    img_infos_sample = []
-    for dataset in datasets:
-        full_list = api.image.get_list(dataset.id)
-
-        marked = [img for img in full_list if img.id in demo_data]
-
-        notmarked = [img_info for img_info in full_list if img_info.labels_count == 0]
-        notmarked = random.sample(notmarked, imagesNotMarked_by_ds[dataset.id])
-
-        img_infos_sample += marked + notmarked
-
-    return img_infos_sample
-
-
-def download_sample_image_project(
-    api,
-    project_id,
-    image_infos: List[sly.ImageInfo],
-    dest_dir,
-    dataset_ids=None,
-    log_progress=False,
-    batch_size=10,
-    only_image_tags=False,
-    save_image_info=False,
-    save_images=True,
-    progress_cb=None,
-):
-    dataset_ids = set(dataset_ids) if (dataset_ids is not None) else None
-    project_fs = Project(dest_dir, OpenMode.CREATE)
-    meta = ProjectMeta.from_json(api.project.get_meta(project_id, with_settings=True))
-    project_fs.set_meta(meta)
-
-    if only_image_tags is True:
-        id_to_tagmeta = meta.tag_metas.get_id_mapping()
-
-    for dataset_info in api.dataset.get_list(project_id):
-        dataset_id = dataset_info.id
-        if dataset_ids is not None and dataset_id not in dataset_ids:
-            continue
-
-        dataset_fs = project_fs.create_dataset(dataset_info.name)
-
-        images = [image for image in image_infos if image.dataset_id == dataset_id]
-
-        ds_progress = None
-        if log_progress:
-            ds_progress = Progress(
-                "Downloading dataset: {!r}".format(dataset_info.name),
-                total_cnt=len(images),
-            )
-
-        for batch in batched(images, batch_size):
-            image_ids = [image_info.id for image_info in batch]
-            image_names = [image_info.name for image_info in batch]
-
-            # download images in numpy format
-            if save_images:
-                batch_imgs_bytes = api.image.download_bytes(dataset_id, image_ids)
-            else:
-                batch_imgs_bytes = [None] * len(image_ids)
-
-            # download annotations in json format
-            if only_image_tags is False:
-                ann_infos = api.annotation.download_batch(dataset_id, image_ids)
-                ann_jsons = [ann_info.annotation for ann_info in ann_infos]
-            else:
-                ann_jsons = []
-                for image_info in batch:
-                    tags = TagCollection.from_api_response(
-                        image_info.tags, meta.tag_metas, id_to_tagmeta
-                    )
-                    tmp_ann = Annotation(
-                        img_size=(image_info.height, image_info.width), img_tags=tags
-                    )
-                    ann_jsons.append(tmp_ann.to_json())
-
-            for img_info, name, img_bytes, ann in zip(
-                batch, image_names, batch_imgs_bytes, ann_jsons
-            ):
-                dataset_fs.add_item_raw_bytes(
-                    item_name=name,
-                    item_raw_bytes=img_bytes if save_images is True else None,
-                    ann=ann,
-                    img_info=img_info if save_image_info is True else None,
+        self._img_height = 1080
+        self._rows = rows
+        self._cols = cols
+        self._row_width = 0
+        self._gap = 15
+        self._bg_color = (221, 210, 230)  # rgb(221, 210, 230)
+        self._side_overlay_path = side_overlay_path
+
+        self._local = False if isinstance(project, int) else True
+        self._api = api if api is not None else sly.Api.from_env()
+
+        self.np_images = []
+        self._img_array = None
+        self._row_height = int((self._img_height - self._gap * (self._rows + 1)) / self._rows)
+
+    @property
+    def basename_stem(self) -> None:
+        return sly.utils.camel_to_snake(self.__class__.__name__)
+
+    def update(self, data: tuple):
+        cnt = self._cols * self._rows
+        join_data = [(ds, img, ann) for ds, list1, list2 in data for img, ann in zip(list1, list2)]
+
+        random.shuffle(join_data)
+        with tqdm(desc="Downloading images", total=cnt) as p:
+            for ds, img_info, ann in join_data[:cnt]:
+                img = (
+                    sly.image.read(ds.get_img_path(img_info.name))
+                    if self._local
+                    else self._api.image.download_np(img_info.id)
                 )
+                mask = self._draw_masks_on_single_image(ann, img_info)
+
+                img = self._resize_image(img)
+                mask = self._resize_image(mask)
+                join_image = np.hstack([img, mask])
+                self.np_images.append(join_image)
+
+                p.update(1)
+
+    def _draw_masks_on_single_image(self, ann: sly.Annotation, image: sly.ImageInfo):
+        height, width = image.height, image.width
+        mask_img = np.zeros((height, width, 3), dtype=np.uint8)
+        mask_img[:, :, 0:3] = self._bg_color  # rgb(221, 210, 230)
+
+        for label in ann.labels:
+            label.geometry.draw(mask_img, color=label.obj_class.color, thickness=3)
+
+        return mask_img
+
+    def to_image(self, path: str = None):
+        path_part, ext = os.path.splitext(path)
+        tmp_path = f"{path_part}-o{ext}"
+        if path is None:
+            storage_dir = sly.app.get_data_dir()
+            path = os.path.join(storage_dir, "horizontal_grid.png")
+
+        self._merge_canvas_with_images()
+        self._add_overlay_with_logo()
+
+        sly.image.write(tmp_path, self._img_array)
+        compress_png(tmp_path, path)
+        sly.fs.silent_remove(tmp_path)
+        sly.logger.info(f"Result grid saved to: {path}")
+
+    def _create_image_canvas(self):
+        self._img_array = np.ones([self._img_height, self._row_width, 3], dtype=np.uint8) * 255
+
+    def _merge_canvas_with_images(self):
+        rows = self._create_rows()
+        self._create_image_canvas()
+        rows = self._merge_img_in_rows(rows)
+        for i, image in enumerate(rows):
+            if image.shape[1] > self._img_array.shape[1]:
+                image = image[:, : self._img_array.shape[1] - self._gap]
+
+            row_start = i * (self._row_height + self._gap) + self._gap
+            row_end = row_start + self._row_height
+            column_start = self._gap
+            column_end = self._img_array.shape[1]
+
+            self._img_array[row_start:row_end, column_start:column_end] = image
+
+    def _create_rows(self):
+        num_images = len(self.np_images)
+        image_widths = [image.shape[1] for image in self.np_images]
+
+        one_big_row_width = sum(image_widths) + (num_images - 1) * self._gap
+        self._row_width = one_big_row_width // self._rows
+
+        rows = []
+        row_images = []
+        current_width = 0
+
+        for image, width in zip(self.np_images, image_widths):
+            if current_width + width > self._row_width:
+                row_images.append(image)
+                rows.append(row_images)
+
+                row_images = []
+                current_width = 0
+
+            row_images.append(image)
+            current_width += width + self._gap
+
+        if len(rows) == self._rows:
+            return rows
+        return rows
+
+    def _merge_img_in_rows(self, rows):
+        combined_rows = []
+        separator = np.ones((self._row_height, 15, 3), dtype=np.uint8) * 255
+        for row in rows:
+            combined_images = []
+
+            for image in row:
+                combined_images.append(image)
+                combined_images.append(separator)
+            combined_images.pop()
+            combined_image = np.hstack(combined_images)
+            combined_rows.append(combined_image)
+
+        return combined_rows
+
+    def _resize_image(self, image):
+        img_h, img_w = image.shape[:2]
+        img_aspect_ratio = self._row_height / img_h
+        img_h = int(self._row_height)
+        img_w = int(img_aspect_ratio * img_w)
+
+        image = sly.image.resize(image, (img_h, img_w))
+
+        return image
+
+    def _add_overlay_with_logo(self):
+        image2 = cv2.imread(self._side_overlay_path, cv2.IMREAD_UNCHANGED)
+        image2 = cv2.cvtColor(image2, cv2.COLOR_BGRA2RGBA)
+
+        _, width1 = self._img_array.shape[:2]
+        height2, width2 = image2.shape[:2]
+
+        alpha_channel = image2[:, :, 3] / 255.0
+
+        x = width1 - width2
 
-            if log_progress:
-                ds_progress.iters_done_report(len(batch))
-            if progress_cb is not None:
-                progress_cb(len(batch))
+        region = self._img_array[:height2, x : x + width2]
+        self._img_array[:height2, x : x + width2, :3] = (
+            1 - alpha_channel[:, :, np.newaxis]
+        ) * region + alpha_channel[:, :, np.newaxis] * image2[:, :, :3]
```

### Comparing `dataset_tools-0.0.85/dataset_tools.egg-info/SOURCES.txt` & `dataset-tools-0.0.9/dataset_tools.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 dataset_tools/__init__.py
+dataset_tools/download.py
 dataset_tools.egg-info/PKG-INFO
 dataset_tools.egg-info/SOURCES.txt
 dataset_tools.egg-info/dependency_links.txt
 dataset_tools.egg-info/requires.txt
 dataset_tools.egg-info/top_level.txt
 dataset_tools/convert/__init__.py
 dataset_tools/convert/cityscapes/__init__.py
 dataset_tools/convert/cityscapes/main.py
 dataset_tools/convert/coco/__init__.py
 dataset_tools/convert/coco/main.py
 dataset_tools/convert/pascal/__init__.py
 dataset_tools/convert/pascal/main.py
-dataset_tools/data/__init__.py
-dataset_tools/data/download_urls/__init__.py
-dataset_tools/data/download_urls/released_datasets.json
-dataset_tools/fonts/FiraSans-Black.ttf
-dataset_tools/fonts/FiraSans-BlackItalic.ttf
-dataset_tools/fonts/FiraSans-Bold.ttf
-dataset_tools/fonts/FiraSans-BoldItalic.ttf
-dataset_tools/fonts/FiraSans-ExtraBold.ttf
-dataset_tools/fonts/FiraSans-ExtraBoldItalic.ttf
-dataset_tools/fonts/FiraSans-ExtraLight.ttf
-dataset_tools/fonts/FiraSans-ExtraLightItalic.ttf
-dataset_tools/fonts/FiraSans-Italic.ttf
-dataset_tools/fonts/FiraSans-Light.ttf
-dataset_tools/fonts/FiraSans-LightItalic.ttf
-dataset_tools/fonts/FiraSans-Medium.ttf
-dataset_tools/fonts/FiraSans-MediumItalic.ttf
-dataset_tools/fonts/FiraSans-Regular.ttf
-dataset_tools/fonts/FiraSans-SemiBold.ttf
-dataset_tools/fonts/FiraSans-SemiBoldItalic.ttf
-dataset_tools/fonts/FiraSans-Thin.ttf
-dataset_tools/fonts/FiraSans-ThinItalic.ttf
 dataset_tools/image/__init__.py
 dataset_tools/image/renders/__init__.py
 dataset_tools/image/renders/convert.py
 dataset_tools/image/renders/horizontal_grid.py
 dataset_tools/image/renders/poster.py
 dataset_tools/image/renders/previews.py
 dataset_tools/image/renders/separated_anns_grid.py
@@ -50,21 +30,11 @@
 dataset_tools/image/stats/class_balance.py
 dataset_tools/image/stats/class_cooccurrence.py
 dataset_tools/image/stats/classes_per_image.py
 dataset_tools/image/stats/heatmaps_for_classes.py
 dataset_tools/image/stats/object_and_class_sizes.py
 dataset_tools/image/stats/objects_distribution.py
 dataset_tools/image/stats/preview_for_classes.py
-dataset_tools/image/stats/tags_cooccurrence.py
 dataset_tools/image/stats/wrapper.py
-dataset_tools/repo/__init__.py
-dataset_tools/repo/download.py
-dataset_tools/repo/project_repo.py
-dataset_tools/repo/sample_project.py
-dataset_tools/templates/__init__.py
-dataset_tools/templates/annotation_types.py
-dataset_tools/templates/applications.py
-dataset_tools/templates/categories.py
-dataset_tools/templates/cv_tasks.py
-dataset_tools/templates/licenses.py
 dataset_tools/text/__init__.py
-dataset_tools/text/generate_summary.py
+dataset_tools/text/summary/__init__.py
+dataset_tools/text/summary/generate.py
```

