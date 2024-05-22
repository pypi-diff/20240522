# Comparing `tmp/vsensebox-0.1.1.tar.gz` & `tmp/vsensebox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsensebox-0.1.1.tar", last modified: Thu May  2 13:26:07 2024, max compression
+gzip compressed data, was "vsensebox-0.2.0.tar", last modified: Wed May 22 14:58:51 2024, max compression
```

## Comparing `vsensebox-0.1.1.tar` & `vsensebox-0.2.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-02 13:25:57.000000 vsensebox-0.1.1/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 13:25:57.000000 vsensebox-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 13:25:57.000000 vsensebox-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-02 13:26:07.386489 vsensebox-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-02 13:25:57.000000 vsensebox-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 13:25:57.000000 vsensebox-0.1.1/RELEASENOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 13:25:58.000000 vsensebox-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.374489 vsensebox-0.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:25:58.000000 vsensebox-0.1.1/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-02 13:25:58.000000 vsensebox-0.1.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:26:07.386489 vsensebox-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-02 13:25:58.000000 vsensebox-0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-02 13:25:58.000000 vsensebox-0.1.1/setup_extra.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.374489 vsensebox-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-02 13:25:58.000000 vsensebox-0.1.1/tests/pretests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 13:25:58.000000 vsensebox-0.1.1/tests/test_01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.374489 vsensebox-0.1.1/vsensebox/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/confighelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/detectors.zip
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/strings/strings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/basiciou.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/centroid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/deepsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/sort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/trackers.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/detectors/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/trackers/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)    53774 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/cfgloader_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/uitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/yolo_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/yolo_ultralytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/basiciou.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox/modules/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/box_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox/vsense/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/vsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/vsense/vsense.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.349582 vsensebox-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-22 14:58:45.000000 vsensebox-0.2.0/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 14:58:45.000000 vsensebox-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 14:58:45.000000 vsensebox-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-22 14:58:51.349582 vsensebox-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-22 14:58:45.000000 vsensebox-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-22 14:58:45.000000 vsensebox-0.2.0/RELEASENOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 14:58:45.000000 vsensebox-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.337581 vsensebox-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-22 14:58:45.000000 vsensebox-0.2.0/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-22 14:58:45.000000 vsensebox-0.2.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:58:51.349582 vsensebox-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-22 14:58:45.000000 vsensebox-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-22 14:58:45.000000 vsensebox-0.2.0/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.337581 vsensebox-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 14:58:45.000000 vsensebox-0.2.0/tests/pretests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 14:58:45.000000 vsensebox-0.2.0/tests/test_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.337581 vsensebox-0.2.0/vsensebox/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.337581 vsensebox-0.2.0/vsensebox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/confighelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.337581 vsensebox-0.2.0/vsensebox/config/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/config/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/detectors.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/config/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/trackers/basiciou.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/trackers/centroid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/trackers/deepsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/trackers/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/trackers/sort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/config/trackers/trackers.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/data/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/data/detectors/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.341582 vsensebox-0.2.0/vsensebox/data/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/data/trackers/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.345582 vsensebox-0.2.0/vsensebox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.345582 vsensebox-0.2.0/vsensebox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    53774 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/gui/cfgloader_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/gui/uitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.345582 vsensebox-0.2.0/vsensebox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.345582 vsensebox-0.2.0/vsensebox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/detectors/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/detectors/yolo_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/detectors/yolo_ultralytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.345582 vsensebox-0.2.0/vsensebox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/basiciou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.349582 vsensebox-0.2.0/vsensebox/modules/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/box_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/modules/trackers/utils/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.349582 vsensebox-0.2.0/vsensebox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/utils/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.349582 vsensebox-0.2.0/vsensebox/vsense/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/vsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-22 14:58:45.000000 vsensebox-0.2.0/vsensebox/vsense/vsense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:51.349582 vsensebox-0.2.0/vsensebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-22 14:58:51.000000 vsensebox-0.2.0/vsensebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-22 14:58:51.000000 vsensebox-0.2.0/vsensebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:58:51.000000 vsensebox-0.2.0/vsensebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-22 14:58:51.000000 vsensebox-0.2.0/vsensebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 14:58:51.000000 vsensebox-0.2.0/vsensebox.egg-info/top_level.txt
```

### Comparing `vsensebox-0.1.1/GETSTARTED.md` & `vsensebox-0.2.0/GETSTARTED.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # 🚀 Getting Started
 
-Installing `VSenseBox` is very easy and straightforward. You can install from [PyPI](https://pypi.org/project/vsensebox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/rathaumons/vsensebox/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependencies or requirements for the modules you need.
+Installing `VSenseBox` is very easy and straightforward. You can install from [PyPI](https://pypi.org/project/vsensebox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/numediart/vsensebox/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependencies or requirements for the modules you need.
 
 ## ⚙️ Requirements
 
 All requirements are not strictly limited. However, some specific modules might need some special dependencies; for example, `YOLO_Classic` (With `.weights` model) runs faster using [OpenCV DNN](https://docs.opencv.org/4.x/d2/d58/tutorial_table_of_content_dnn.html) with GPU. In this case, you might need to build OpenCV from source with GPU support or use our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) instead of the official `opencv-contrib-python`.
 
 * Prerequisite: 
   - Python [[3.9-3.12]](https://www.python.org/downloads/)
-  - Local `VSenseBox` repo: `git clone https://github.com/rathaumons/vsensebox.git`
+  - Local `VSenseBox` repo: `git clone https://github.com/numediart/vsensebox.git`
 
 * Before you install dependencies/requirements:
   - For Linux, recommend changing `python3` to `python`: `sudo apt install python-is-python3`
   - If you prefer conda + Python [3.9-3.12]: `conda create --name vsensebox_env python=3.11`
   - Upgrade `pip` and `setuptools`:
     ```
     python -m pip install --upgrade pip
@@ -51,59 +51,59 @@
     - For CPU:
       ```
       pip install torch torchvision torchaudio
       pip install -r requirements.txt
       ```
 
 * ***ATTENTION ⚠️⚠️⚠️***
-  - Default configurations of `VSenseBox` are set to use GPU, and to switch to CPU, you need to set `cpu` as string for the parameter `device` in the YAML config file; for example, line #8 in [`yolo_ultralytics_v9c.yaml`](https://github.com/rathaumons/vsensebox/blob/main/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml).
+  - Default configurations of `VSenseBox` are set to use GPU, and to switch to CPU, you need to set `cpu` as string for the parameter `device` in the YAML config file; for example, line #8 in [`yolo_ultralytics_v9c.yaml`](https://github.com/numediart/vsensebox/blob/main/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml).
 
 
 ## 💽 Setup
 
 `vsensebox` is the main package and if you use the classic YOLO detectors and DeepSORT tracker, etc., you need to also install `vsensebox-data-xxx`.
 
 * Install `vsensebox`
-  - Download and install the latest wheel in GitHub [releases](https://github.com/rathaumons/vsensebox/releases) or install from [PyPI](https://pypi.org/project/vsensebox/):
+  - Download and install the latest wheel in GitHub [releases](https://github.com/numediart/vsensebox/releases) or install from [PyPI](https://pypi.org/project/vsensebox/):
     ```
     pip install vsensebox
     ``` 
   - Or install directly from GitHub:
     ```
-    pip install git+https://github.com/rathaumons/vsensebox.git
+    pip install git+https://github.com/numediart/vsensebox.git
     ```
   - Or build from source:
     ```
     pip install wheel build PyYAML
     python -m build --wheel --skip-dependency-check --no-isolation
     ```
 
-* Install [`vsensebox-data-xxx`](https://github.com/rathaumons/vsensebox-data/)
-  - Download the latest from GitHub [releases](https://github.com/rathaumons/vsensebox-data/releases) and install
+* Install [`vsensebox-data-xxx`](https://github.com/numediart/vsensebox-data/)
+  - Download the latest from GitHub [releases](https://github.com/numediart/vsensebox-data/releases) and install
   - Or install the ones you need directly from the links below:
     ```
-    pip install https://github.com/rathaumons/vsensebox-data/releases/download/v0.0.0/vsensebox_data_yolocls-0.0.0-py3-none-any.whl
-    pip install https://github.com/rathaumons/vsensebox-data/releases/download/v0.0.0/vsensebox_data_yoloult-0.0.0-py3-none-any.whl
-    pip install https://github.com/rathaumons/vsensebox-data/releases/download/v0.0.0/vsensebox_data_deepsort-0.0.0-py3-none-any.whl
+    pip install https://github.com/numediart/vsensebox-data/releases/download/v0.0.0/vsensebox_data_yolocls-0.0.0-py3-none-any.whl
+    pip install https://github.com/numediart/vsensebox-data/releases/download/v0.0.0/vsensebox_data_yoloult-0.0.0-py3-none-any.whl
+    pip install https://github.com/numediart/vsensebox-data/releases/download/v0.0.0/vsensebox_data_deepsort-0.0.0-py3-none-any.whl
     ```
 
 * Let's try some basic features of `VSenseBox`
   - Configurator GUI can be called in Python terminal:
     ```
     import vsensebox
     vsensebox.config()
     ```
     Now you should see the Configurator GUI like in this scheenshot:
     <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/VSenseBox/vsensebox_config_gui.jpg">
   - You can also easily reset the internal configurations by calling the `reset()`. **THIS CAN'T BE REVERSED!** ⚠️
     ```
     vsensebox.reset()
     ```
-  - For the details of GUI functions and configurations, check [Configurations page](https://rathaumons.github.io/vsensebox/vsensebox/config.html).
-  - Check the [Examples page](https://rathaumons.github.io/vsensebox/examples.html) for some real coding!
+  - For the details of GUI functions and configurations, check [Configurations page](https://numediart.github.io/vsensebox/vsensebox/config.html).
+  - Check the [Examples page](https://numediart.github.io/vsensebox/examples.html) for some real coding!
 * For ***Linux***, if the GUI does not work, you might need to install these:
   ```
   sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev
   ```
 * For ***Ubuntu on WSL 2***, if the GUI does not work, you need to install these:
   ```
   sudo apt-get install libgl1-mesa-glx
@@ -115,8 +115,8 @@
 
 ### 1️⃣ Customized OpenCV
 
 OpenCV is widely used in many well-known packages, but the majority of the prebuilt WHLs on the Internet including the official one on PyPI do not include GPU support. Thus, we build our custom one which includes NVIDIA [CUDA](https://developer.nvidia.com/cuda-downloads) & [cuDNN](https://developer.nvidia.com/rdp/cudnn-download) supports for the [OpenCV DNN module](https://docs.opencv.org/4.x/d2/d58/tutorial_table_of_content_dnn.html). In order to well distinguish from the rest, we decided to build and change the package name from `opencv-contrib-python` to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) -> [[Repo]](https://github.com/rathaumons/opencv-for-pyppbox) [[WHL]](https://github.com/rathaumons/opencv-for-pyppbox/releases)
 
 ### 2️⃣ Customized Ultralytics
 
-Also, similar to `pyppbox-opencv`, our custom `ultralytics` is changed to [`vsensebox-ultralytics`](https://github.com/rathaumons/ultralytics-for-vsensebox), but this time, the module name is still the same `ultralytics` and it is the main reason why the official `ultralytics` must be removed. Find out more why `VSenseBox` needs the customized `vsensebox-ultralytics` -> [[Repo]](https://github.com/rathaumons/ultralytics-for-vsensebox) [[PyPI]](https://pypi.org/project/vsensebox-ultralytics/)
+Also, similar to `pyppbox-opencv`, our custom `ultralytics` is changed to [`vsensebox-ultralytics`](https://github.com/numediart/ultralytics-for-vsensebox), but this time, the module name is still the same `ultralytics` and it is the main reason why the official `ultralytics` must be removed. Find out more why `VSenseBox` needs the customized `vsensebox-ultralytics` -> [[Repo]](https://github.com/numediart/ultralytics-for-vsensebox) [[PyPI]](https://pypi.org/project/vsensebox-ultralytics/)
```

### Comparing `vsensebox-0.1.1/LICENSE` & `vsensebox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/PKG-INFO` & `vsensebox-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.1.1
+Version: 0.2.0
 Summary: VSenseBox - Python toolbox for visual sensing.
-Home-page: https://github.com/rathaumons/vsensebox
+Home-page: https://github.com/numediart/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -45,29 +45,29 @@
 Requires-Dist: future
 Requires-Dist: protobuf
 Requires-Dist: tensorflow
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: filterpy
-Requires-Dist: lapx>=0.5.8
+Requires-Dist: lapx>=0.5.9
 Requires-Dist: PyQt6
 Requires-Dist: vsensebox-ultralytics>=8.1.48
 
-# 👁️📦 [**VSenseBox**](https://github.com/rathaumons/vsensebox)
+# 👁️📦 [**VSenseBox**](https://github.com/numediart/vsensebox)
 
 <div align="center">
 
-[![Documentation](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml)
+[![Documentation](https://github.com/numediart/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/numediart/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/numediart/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_build.yaml)
 
-[![Test Windows](https://github.com/rathaumons/vsensebox/actions/workflows/test_windows.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_windows.yaml) [![Test Linux](https://github.com/rathaumons/vsensebox/actions/workflows/test_linux.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_linux.yaml) [![Test macOS](https://github.com/rathaumons/vsensebox/actions/workflows/test_macos.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_macos.yaml)
+[![Test Windows](https://github.com/numediart/vsensebox/actions/workflows/test_windows.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_windows.yaml) [![Test Linux](https://github.com/numediart/vsensebox/actions/workflows/test_linux.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_linux.yaml) [![Test macOS](https://github.com/numediart/vsensebox/actions/workflows/test_macos.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_macos.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/VSenseBox/vsensebox.jpg"><br />
 
-**[📗 Documentation](https://rathaumons.github.io/vsensebox/) | [🚀 Getting started](https://rathaumons.github.io/vsensebox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/vsensebox/examples.html)**
+**[📗 Documentation](https://numediart.github.io/vsensebox/) | [🚀 Getting started](https://numediart.github.io/vsensebox/getstarted.html) | [💡 Examples](https://numediart.github.io/vsensebox/examples.html)**
 
 </div>
 
 ***VSenseBox*** is a small all-in-one Python toolbox filled with many vision/visual sensing modules such as object detectors and object trackers, etc. These modules are well integrated together and can be easily selected and configurated with minimal coding.
 
 * Integrate with popular object detectors including YOLO v3, v4, v5, v8, v9, and more.
 * Integrate with bbox trackers including Centroid, SORT, DeepSORT, and more TBA.
```

### Comparing `vsensebox-0.1.1/README.md` & `vsensebox-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# 👁️📦 [**VSenseBox**](https://github.com/rathaumons/vsensebox)
+# 👁️📦 [**VSenseBox**](https://github.com/numediart/vsensebox)
 
 <div align="center">
 
-[![Documentation](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml)
+[![Documentation](https://github.com/numediart/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/numediart/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/numediart/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_build.yaml)
 
-[![Test Windows](https://github.com/rathaumons/vsensebox/actions/workflows/test_windows.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_windows.yaml) [![Test Linux](https://github.com/rathaumons/vsensebox/actions/workflows/test_linux.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_linux.yaml) [![Test macOS](https://github.com/rathaumons/vsensebox/actions/workflows/test_macos.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_macos.yaml)
+[![Test Windows](https://github.com/numediart/vsensebox/actions/workflows/test_windows.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_windows.yaml) [![Test Linux](https://github.com/numediart/vsensebox/actions/workflows/test_linux.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_linux.yaml) [![Test macOS](https://github.com/numediart/vsensebox/actions/workflows/test_macos.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_macos.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/VSenseBox/vsensebox.jpg"><br />
 
-**[📗 Documentation](https://rathaumons.github.io/vsensebox/) | [🚀 Getting started](https://rathaumons.github.io/vsensebox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/vsensebox/examples.html)**
+**[📗 Documentation](https://numediart.github.io/vsensebox/) | [🚀 Getting started](https://numediart.github.io/vsensebox/getstarted.html) | [💡 Examples](https://numediart.github.io/vsensebox/examples.html)**
 
 </div>
 
 ***VSenseBox*** is a small all-in-one Python toolbox filled with many vision/visual sensing modules such as object detectors and object trackers, etc. These modules are well integrated together and can be easily selected and configurated with minimal coding.
 
 * Integrate with popular object detectors including YOLO v3, v4, v5, v8, v9, and more.
 * Integrate with bbox trackers including Centroid, SORT, DeepSORT, and more TBA.
```

### Comparing `vsensebox-0.1.1/RELEASENOTES.md` & `vsensebox-0.2.0/RELEASENOTES.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 # Release Notes 
 
+## **VSenseBox v0.2.x - Some Changes!**
+
+* `VSenseBox` [v0.2.0](https://github.com/numediart/vsensebox/tree/v0.2.0)
+  - Transfer from [rathaumons](https://github.com/rathaumons) to [numediart](https://github.com/numediart)
+  - Change `boxes_confs` to `boxes_conf` for `VSenseAssets`
+  - Update requirements
+  - Update and improve documentation
+
 ## **VSenseBox v0.1.x - One Small Step!**
 
-* `VSenseBox` [v0.1.1](https://github.com/rathaumons/vsensebox/tree/v0.1.1)
-  - Replace [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox) with [`vsensebox-ultralytics`](https://github.com/rathaumons/ultralytics-for-vsensebox)
+* `VSenseBox` [v0.1.1](https://github.com/numediart/vsensebox/tree/v0.1.1)
+  - Replace [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox) with [`vsensebox-ultralytics`](https://github.com/numediart/ultralytics-for-vsensebox)
   - Use `lapx>=0.5.8` for speed boost
   - Update and improve documentation
   - Update GitHub workflow
 
-* `VSenseBox` [v0.1.0](https://github.com/rathaumons/vsensebox/tree/v0.1.0)
+* `VSenseBox` [v0.1.0](https://github.com/numediart/vsensebox/tree/v0.1.0)
   - Add basic IoU tracker -> `BasicIoU`
   - Fix minor bugs
   - Clean up and improve unified strings
   - Update and improve configurator and GUI
   - Update and improve documentation
 
 ## **VSenseBox v0.0.x - Hello World!**
 
-* `VSenseBox` [v0.0.4](https://github.com/rathaumons/vsensebox/tree/v0.0.4)
+* `VSenseBox` [v0.0.4](https://github.com/numediart/vsensebox/tree/v0.0.4)
   - Add minor bug fixes
   - Add example 03 for multithreading
   - Improve overall performance
   - Update and improve documentation
 
-* `VSenseBox` [v0.0.3](https://github.com/rathaumons/vsensebox/tree/v0.0.3)
+* `VSenseBox` [v0.0.3](https://github.com/numediart/vsensebox/tree/v0.0.3)
   - Improve `VSense` performance
   - Update and improve documentation
 
-* `VSenseBox` [v0.0.2](https://github.com/rathaumons/vsensebox/tree/v0.0.2)
+* `VSenseBox` [v0.0.2](https://github.com/numediart/vsensebox/tree/v0.0.2)
   - Add direct YAML file reading to `config()`
   - Update and improve documentation
 
-* `VSenseBox` [v0.0.1](https://github.com/rathaumons/vsensebox/tree/v0.0.1)
+* `VSenseBox` [v0.0.1](https://github.com/numediart/vsensebox/tree/v0.0.1)
   - Fix the wrong paths in yolo_classic *.yaml
 
-* `VSenseBox` [v0.0.0](https://github.com/rathaumons/vsensebox/tree/v0.0.0)
+* `VSenseBox` [v0.0.0](https://github.com/numediart/vsensebox/tree/v0.0.0)
   - Initialize first release 👋
-  - Come with full [documentation](https://rathaumons.github.io/vsensebox/) 📄
+  - Come with full [documentation](https://numediart.github.io/vsensebox/) 📄
   - Support both CPU and GPU ready 🚀
   - Support Python 3.9-3.12 on Windows, Linux, and macOS 🫶
   - Support multithreading 🛞
   - Support YAML config file ✍️
   - Integrate with PyQt GUI for easy config 🖱️
   - Integrate with object detectors and trackers 🤖
     - Built-in Classic YOLO v3 and v4 (.weights models)
```

### Comparing `vsensebox-0.1.1/requirements/requirements.txt` & `vsensebox-0.2.0/requirements/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-### FOR MORE DETAILS -> VISIT https://rathaumons.github.io/vsensebox/getstarted.html
+### FOR MORE DETAILS -> VISIT https://numediart.github.io/vsensebox/getstarted.html
 ### Base
 Cython>=0.29.33
 numpy
 ### OpenCV
 # For GPU support, check:
 # https://github.com/rathaumons/opencv-for-pyppbox
 opencv-contrib-python
@@ -25,12 +25,12 @@
 # Please follow the installation on:
 # https://pytorch.org/get-started
 torch
 torchvision
 torchaudio
 ### Tracker: SORT
 filterpy
-lapx>=0.5.8
+lapx>=0.5.9
 ### GUI
 PyQt6
 ### Customized vsensebox-ultralytics
 vsensebox-ultralytics>=8.1.48
```

### Comparing `vsensebox-0.1.1/setup.py` & `vsensebox-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def main_setup():
     long_description = open("README.md", encoding="utf-8").read()
     packages, package_data = get_packages()
     setup(
         name="vsensebox",
         version=get_version_string(),
-        url="https://github.com/rathaumons/vsensebox",
+        url="https://github.com/numediart/vsensebox",
         license="GPL-3.0-or-later",
         description="VSenseBox - Python toolbox for visual sensing.",
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=packages,
         package_data=package_data,
         include_package_data=True,
```

### Comparing `vsensebox-0.1.1/setup_extra.yaml` & `vsensebox-0.2.0/setup_extra.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/tests/pretests.py` & `vsensebox-0.2.0/tests/pretests.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/tests/test_01.py` & `vsensebox-0.2.0/tests/test_01.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         # Track object using internal YAML config file
         vs.track(img=frame, img_is_mat=True)
         
         # Draw bounding boxes of the detected objects
         frame = draw_boxes(
             frame, ids=vs.assets.ids, 
             boxes_xyxy=vs.assets.boxes_xyxy, 
-            boxes_confs=vs.assets.boxes_confs
+            boxes_conf=vs.assets.boxes_conf
         )
 
         # Save frame as jpg
         cv2.imwrite("tests_outputs/test_01_frame_" + str(frame_index) + ".jpg", frame)
         frame_index += 1
 
         if frame_index == stop_after:
```

### Comparing `vsensebox-0.1.1/vsensebox/__init__.py` & `vsensebox-0.2.0/vsensebox/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 from vsensebox.vsense import VSense
 from vsensebox.gui import config, reset
 from vsensebox.utils.about import docs, github
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __author__ = "Ratha SIV"
 __description__ = "VSenseBox - Python toolbox for visual sensing."
-__homepage__ = "https://rathaumons.github.io/vsensebox"
-__url__ = "https://github.com/rathaumons/vsensebox.git"
+__homepage__ = "https://numediart.github.io/vsensebox"
+__url__ = "https://github.com/numediart/vsensebox.git"
 
 __all__ = (
     "__version__", 
     "VSense", 
     "config", 
     "reset", 
     "docs",
```

### Comparing `vsensebox-0.1.1/vsensebox/config/confighelper.py` & `vsensebox-0.2.0/vsensebox/config/confighelper.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/config/configurator.py` & `vsensebox-0.2.0/vsensebox/config/configurator.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/config/detectors/detectors.zip` & `vsensebox-0.2.0/vsensebox/config/detectors/detectors.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/config/strings.py` & `vsensebox-0.2.0/vsensebox/config/strings.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/config/trackers/trackers.zip` & `vsensebox-0.2.0/vsensebox/config/trackers/trackers.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/gui/assets/settings.ico` & `vsensebox-0.2.0/vsensebox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/gui/cfgloader_ui.py` & `vsensebox-0.2.0/vsensebox/gui/cfgloader_ui.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/gui/uitools.py` & `vsensebox-0.2.0/vsensebox/gui/uitools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/detectors/detectors.py` & `vsensebox-0.2.0/vsensebox/modules/detectors/detectors.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,27 @@
 
 from vsensebox.config.strings import USTR
 from vsensebox.config.confighelper import getCFGDict
 from vsensebox.config.configurator import DCFG_YOLOULT, DCFG_YOLOCLS
 
 
 def checkDet(detector, config_yaml, relative_to_vsensebox_root):
-    
+    """Automatically check, select, and config the supported detector according to the 
+    input :obj:`config_yaml`.
+
+    Parameters
+    ----------
+    detector : detector object
+        A detector object; for example, :class:`YOLO_Ultralytics` or :class:`YOLO_Classic`.
+    config_yaml : str or dict
+        A YAML/JSON file path, or a raw/ready dictionary.
+    relative_to_vsensebox_root : bool
+        This parameter is passed to the corresponding configurator; for example, 
+        :class:`DCFG_YOLOULT` or :class:`DCFG_YOLOCLS`.
+    """
     cfg = getCFGDict(config_yaml)
     det_name = USTR.getUnifiedFormat(cfg['detector'])
 
     if detector is None:
         from .yolo_ultralytics import YOLO_Ultralytics
         from .yolo_classic import YOLO_Classic
         detectors = {
```

### Comparing `vsensebox-0.1.1/vsensebox/modules/detectors/yolo_classic.py` & `vsensebox-0.2.0/vsensebox/modules/detectors/yolo_classic.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/detectors/yolo_ultralytics.py` & `vsensebox-0.2.0/vsensebox/modules/detectors/yolo_ultralytics.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/basiciou.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/basiciou.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,22 +64,22 @@
             if iou > max_iou and self.prev_cls[i] == box_class:
                 max_iou = iou
                 pindex = i
             i += 1
         if max_iou < self.min_iou: pindex = -1
         return pindex
 
-    def update(self, boxes_xyxy, boxes_confs, boxes_cls=None, img=None):
+    def update(self, boxes_xyxy, boxes_conf, boxes_cls=None, img=None):
         """Update the tracker and return a track list.
 
         Parameters
         ----------
         boxes_xyxy : list[[X1, Y1, X2, Y2], ...]
             A list of boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
-        boxes_confs : list[float, ...]
+        boxes_conf : list[float, ...]
             Being consistent with other trackers, will be ignored.
         boxes_cls : list[int, ...], default=None
             A list of detection class corresponding to boxes_xyxy.
         img : any, default=None
             Being consistent with other trackers, will be ignored.
 
         Returns
```

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/centroid.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/centroid.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,22 +53,22 @@
             if d < min_d:
                 min_d = d
                 pindex = i
             i += 1
         if min_d > self.max_spread: pindex = -1
         return pindex
 
-    def update(self, boxes_xyxy, boxes_confs, boxes_cls=None, img=None):
+    def update(self, boxes_xyxy, boxes_conf, boxes_cls=None, img=None):
         """Update the tracker and return a track list.
 
         Parameters
         ----------
         boxes_xyxy : list[[X1, Y1, X2, Y2], ...]
             A list of boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
-        boxes_confs : list[float, ...]
+        boxes_conf : list[float, ...]
             Being consistent with other trackers, will be ignored.
         boxes_cls : list[int, ...], default=None
             Being consistent with other trackers, will be ignored.
         img : any, default=None
             Being consistent with other trackers, will be ignored.
 
         Returns
```

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/deepsort.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/deepsort.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,37 +40,37 @@
         self.encoder = gdet.create_box_encoder(cfg.model_file, batch_size=cfg.batch_size)
         self.metric = nn_matching.NearestNeighborDistanceMetric(
             "cosine", cfg.max_cosine_distance,cfg.nn_budget
         )
         self.tracker = DSTracker(self.metric)
 
 
-    def update(self, boxes_xyxy, boxes_confs, boxes_cls=None, img=None):
+    def update(self, boxes_xyxy, boxes_conf, boxes_cls=None, img=None):
         """Update the tracker and return a track list.
 
         Parameters
         ----------
         boxes_xyxy : list[[X1, Y1, X2, Y2], ...]
             A list of boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
-        boxes_confs : list[float, ...]
+        boxes_conf : list[float, ...]
             A list of detection confidences corresponding to boxes_xyxy.
         boxes_cls : list[int, ...], default=None
             A list of detection class corresponding to boxes_xyxy.
         img : any, default=None
             A :obj:`Mat` like object.
 
         Returns
         -------
         list[[X1, Y1, X2, Y2], ...]
             A list of boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
         list[int]
             A list of IDs corresponding to the the list of boxes.
         """
 
-        dconfidences = boxes_confs
+        dconfidences = boxes_conf
         dclasses = boxes_cls
         dboxes = [to_xywh(b) for b in boxes_xyxy]
         dfeatures = self.encoder(img, dboxes)
         detections = [DSDetection(dbox, dconfidence, dclass, dfeature) 
                         for dbox, dconfidence, dclass, dfeature in 
                         zip(dboxes, dconfidences, dclasses, dfeatures)]
         dboxes = np.array([d.tlwh for d in detections])
```

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/sort.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/sort.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,35 +22,35 @@
         Parameters
         ----------
         cfg : TCFG_SORT
           A :class:`TCFG_SORT` object which manages the configurations of tracker SORT.
         """
         self.st = ST(cfg.max_age, cfg.min_hits, cfg.iou_threshold)
 
-    def update(self, boxes_xyxy, boxes_confs, boxes_cls=None, img=None):
+    def update(self, boxes_xyxy, boxes_conf, boxes_cls=None, img=None):
         """Update the tracker and return a track list.
 
         Parameters
         ----------
         boxes_xyxy : list[[X1, Y1, X2, Y2], ...]
           A list of boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
-        boxes_confs : list[float, ...]
+        boxes_conf : list[float, ...]
           A list of detection confidence corresponding to boxes_xyxy.
         boxes_cls : list[int, ...], default=None
           Being consistent with other trackers, will be ignored.
         img : any, default=None
           Being consistent with other trackers, will be ignored.
 
         Returns
         -------
         list[[X1, Y1, X2, Y2], ...]
             A list of boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
         list[int]
             A list of IDs corresponding to the the list of boxes.
         """
         detection = []
-        for b, c in zip(boxes_xyxy, boxes_confs):
+        for b, c in zip(boxes_xyxy, boxes_conf):
           b = np.append(b, c)
           detection.append(b)
         track = self.st.update(np.array(detection)).astype(int)
         ids = matchDetTrkByXYXYForSORT(boxes_xyxy, track, max_spread=10)
         return boxes_xyxy, ids
```

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/box_matching.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/box_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/detection.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection_yolo.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/generate_detections.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/generate_detections.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/iou_matching.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/iou_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/kalman_filter.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/linear_assignment.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/nn_matching.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/nn_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/preprocessing.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/sort.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/track.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/track.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/modules/trackers/utils/tracker.py` & `vsensebox-0.2.0/vsensebox/modules/trackers/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/utils/about.py` & `vsensebox-0.2.0/vsensebox/utils/about.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             raise RuntimeError(msg)
 
 def github():
     """
     :meta private:
     """
     import webbrowser
-    webbrowser.open('https://github.com/rathaumons/vsensebox.git')
+    webbrowser.open('https://github.com/numediart/vsensebox.git')
 
 def docs():
     """
     :meta private:
     """
     import webbrowser
-    webbrowser.open('https://rathaumons.github.io/vsensebox')
+    webbrowser.open('https://numediart.github.io/vsensebox')
```

### Comparing `vsensebox-0.1.1/vsensebox/utils/commontools.py` & `vsensebox-0.2.0/vsensebox/utils/commontools.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 import os
 import sys
 import cv2
 import numpy as np
 
-
 def getCVMat(img, to_rgb=False):
     """
     :meta private:
     """
     if isinstance(img, str):
         if isExist(img):
             try:
```

### Comparing `vsensebox-0.1.1/vsensebox/utils/logtools.py` & `vsensebox-0.2.0/vsensebox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.1/vsensebox/utils/visualizetools.py` & `vsensebox-0.2.0/vsensebox/utils/visualizetools.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .commontools import getCVMat
 from .logtools import add_warning_log
 
 def draw_boxes(img, 
                ids=[], 
                show_ids=True, 
                boxes_xyxy=[], 
-               boxes_confs=[], 
+               boxes_conf=[], 
                boxes_color=(255, 255, 0), 
                boxes_thickness=2, 
                text_color=(150, 200, 50), 
                text_font=cv2.FONT_HERSHEY_COMPLEX_SMALL, 
                text_font_scale=1, 
                text_thickness=1, 
                img_is_mat=True):
@@ -26,15 +26,15 @@
     ----------
     img : str or Mat
         An image file or a :obj:`Mat` like object.
     show_ids : bool, default=True
         Whether to visualize the IDs.
     boxes_xyxy : list[[X1, Y1, X2, Y2], ...], default=[]
         A list of bounding boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
-    boxes_confs : list[float, ...], default=[]
+    boxes_conf : list[float, ...], default=[]
         A list of detection confidences corresponding to bounding boxes.
     boxes_color : tuple(int, int, int), default=(255, 255, 0)
         Color space of bounding boxes.
     boxes_thickness : int, default=2
         Thickness of bounding boxes.
     text_color : tuple(int, int, int), default=(150, 200, 50)
         Color space of the texts for IDs and confs.
@@ -65,15 +65,15 @@
             img, 
             (int(boxes_xyxy[i][0]), int(boxes_xyxy[i][1])), (int(boxes_xyxy[i][2]), int(boxes_xyxy[i][3])), 
             boxes_color, 
             boxes_thickness
         )
         conf = 0.0
         try:
-            conf = format(boxes_confs[i], '.2f')
+            conf = format(boxes_conf[i], '.2f')
             cv2.putText(img, str(conf), (int(boxes_xyxy[i][0]) + 5, int(boxes_xyxy[i][3]) - 5), 
                         text_font, text_font_scale, text_color, text_thickness)
         except Exception as e:
             add_warning_log("VSenseBox:draw_boxes() -> Numbers of confs and boxes are different!")
         if show_ids: 
             cv2.putText(img, "#" + str(ids[i]), (int(boxes_xyxy[i][0]), int(boxes_xyxy[i][1] - 5)), 
                         text_font, text_font_scale, text_color, text_thickness)
```

### Comparing `vsensebox-0.1.1/vsensebox/vsense/vsense.py` & `vsensebox-0.2.0/vsensebox/vsense/vsense.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 DEFAULT_TRK_CONFIG = getCFGDict(joinFPathFull(TRK_CONFIG_DIR, 'default.yaml'))
 DEFAULT_TRK_YAML = joinFPathFull(IN_ROOT_DIR, DEFAULT_TRK_CONFIG['config_yaml'])
 TRK_YAML_TO_ROOT = True if getAncestorDir(DEFAULT_TRK_CONFIG['config_yaml']) == 'config/trackers' else False
 
 
 class VSense(object):
 
-    """
-    VSense is used to operate the object detection and tracking.
+    """VSense is used to operate the object detection and tracking.
 
     Attributes
     ----------
     assets : VSenseAssets
         A :class:`VSenseAssets` object used to store assets of VSense.
     """
 
@@ -65,15 +64,15 @@
         else:
             self._yaml_det = config_yaml
         img, boxes_xywh, boxes_xyxy, keypoints, confs, cls = self._detector.detect(img)
         self.assets.update(
             boxes_xywh=boxes_xywh, 
             boxes_xyxy=boxes_xyxy, 
             keypoints=keypoints, 
-            boxes_confs=confs,
+            boxes_conf=confs,
             boxes_cls=cls
         )
 
     def track(self, img=None, config_yaml=None, img_is_mat=False):
         """Track the detected objects in the given image :obj:`img`.
 
         Parameters
@@ -92,15 +91,15 @@
         if self._yaml_trk != config_yaml:
             self._tracker = checkTrk(tracker=self._tracker, config_yaml=config_yaml, 
                                      relative_to_vsensebox_root=self._trk_rel_to_root)
         else:
             self._yaml_trk = config_yaml
         boxes_xyxy, self.assets.ids = self._tracker.update(
             self.assets.boxes_xyxy, 
-            self.assets.boxes_confs, 
+            self.assets.boxes_conf, 
             boxes_cls=self.assets.boxes_cls, 
             img=img
         )
 
 
 class VSenseAssets(object):
     
@@ -109,15 +108,15 @@
 
     Attributes
     ----------
     boxes_xyxy : list[[X1, Y1, X2, Y2], ...], optional
         A list of bounding boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
     boxes_xywh : list[[X, Y, W, H], ...], optional
         A list of bounding boxes; for example, [[X, Y, W, H], [X, Y, W, H], ...].
-    boxes_confs : list[float, ...], optional
+    boxes_conf : list[float, ...], optional
         A list of detection confidences corresponding to bounding boxes.
     boxes_cls : list[int, ...], optional
         A list of detection class corresponding to bounding boxes.
     keypoints : list[], optional
         A list of detected bodies' keypoints.
     ids: list[int, ...], optional
         A list of IDs corresponding to bounding boxes.
@@ -128,53 +127,53 @@
     """
     
     def __init__(self):
         """Construct a VSenseAssets.
         """
         self.boxes_xyxy = []
         self.boxes_xywh = []
-        self.boxes_confs = []
+        self.boxes_conf = []
         self.boxes_cls = []
         self.keypoints = []
         self.ids = []
         self.masks = []
         self.miscs = []
     
     def update(self, 
                boxes_xyxy=[], 
                boxes_xywh=[], 
-               boxes_confs=[], 
+               boxes_conf=[], 
                boxes_cls=[], 
                keypoints=[], 
                ids=[], 
                masks=[], 
                miscs=[]):
         """Update a VSenseAssets.
 
         Parameters
         ----------
         boxes_xyxy : list[[X1, Y1, X2, Y2], ...], optional
             A list of bounding boxes; for example, [[X1, Y1, X2, Y2], [X1, Y1, X2, Y2], ...].
         boxes_xywh : list[[X, Y, W, H], ...], optional
             A list of bounding boxes; for example, [[X, Y, W, H], [X, Y, W, H], ...].
-        boxes_confs : list[float, ...], optional
+        boxes_conf : list[float, ...], optional
             A list of detection confidences corresponding to bounding boxes.
         boxes_cls : list[int, ...], optional
             A list of detection class corresponding to bounding boxes.
         keypoints : list[], optional
             A list of detected bodies' keypoints.
         ids: list[int, ...], optional
             A list of IDs corresponding to bounding boxes.
         masks: list[], optional
             A list of detected masks.
         misc : list[], optional
             A list of miscellaneous items.
         """
         self.boxes_xyxy = boxes_xyxy
         self.boxes_xywh = boxes_xywh
-        self.boxes_confs = boxes_confs
+        self.boxes_conf = boxes_conf
         self.boxes_cls = boxes_cls
         self.keypoints = keypoints
         self.ids = ids
         self.masks = masks
         self.miscs = miscs
```

### Comparing `vsensebox-0.1.1/vsensebox.egg-info/PKG-INFO` & `vsensebox-0.2.0/vsensebox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.1.1
+Version: 0.2.0
 Summary: VSenseBox - Python toolbox for visual sensing.
-Home-page: https://github.com/rathaumons/vsensebox
+Home-page: https://github.com/numediart/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -45,29 +45,29 @@
 Requires-Dist: future
 Requires-Dist: protobuf
 Requires-Dist: tensorflow
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: filterpy
-Requires-Dist: lapx>=0.5.8
+Requires-Dist: lapx>=0.5.9
 Requires-Dist: PyQt6
 Requires-Dist: vsensebox-ultralytics>=8.1.48
 
-# 👁️📦 [**VSenseBox**](https://github.com/rathaumons/vsensebox)
+# 👁️📦 [**VSenseBox**](https://github.com/numediart/vsensebox)
 
 <div align="center">
 
-[![Documentation](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml)
+[![Documentation](https://github.com/numediart/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/numediart/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/numediart/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_build.yaml)
 
-[![Test Windows](https://github.com/rathaumons/vsensebox/actions/workflows/test_windows.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_windows.yaml) [![Test Linux](https://github.com/rathaumons/vsensebox/actions/workflows/test_linux.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_linux.yaml) [![Test macOS](https://github.com/rathaumons/vsensebox/actions/workflows/test_macos.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_macos.yaml)
+[![Test Windows](https://github.com/numediart/vsensebox/actions/workflows/test_windows.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_windows.yaml) [![Test Linux](https://github.com/numediart/vsensebox/actions/workflows/test_linux.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_linux.yaml) [![Test macOS](https://github.com/numediart/vsensebox/actions/workflows/test_macos.yaml/badge.svg)](https://github.com/numediart/vsensebox/actions/workflows/test_macos.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/VSenseBox/vsensebox.jpg"><br />
 
-**[📗 Documentation](https://rathaumons.github.io/vsensebox/) | [🚀 Getting started](https://rathaumons.github.io/vsensebox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/vsensebox/examples.html)**
+**[📗 Documentation](https://numediart.github.io/vsensebox/) | [🚀 Getting started](https://numediart.github.io/vsensebox/getstarted.html) | [💡 Examples](https://numediart.github.io/vsensebox/examples.html)**
 
 </div>
 
 ***VSenseBox*** is a small all-in-one Python toolbox filled with many vision/visual sensing modules such as object detectors and object trackers, etc. These modules are well integrated together and can be easily selected and configurated with minimal coding.
 
 * Integrate with popular object detectors including YOLO v3, v4, v5, v8, v9, and more.
 * Integrate with bbox trackers including Centroid, SORT, DeepSORT, and more TBA.
```

### Comparing `vsensebox-0.1.1/vsensebox.egg-info/SOURCES.txt` & `vsensebox-0.2.0/vsensebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

