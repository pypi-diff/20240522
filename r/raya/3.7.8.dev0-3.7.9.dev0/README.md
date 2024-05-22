# Comparing `tmp/raya-3.7.8.dev0.tar.gz` & `tmp/raya-3.7.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-3.7.8.dev0.tar", last modified: Mon Jan 22 23:06:31 2024, max compression
+gzip compressed data, was "raya-3.7.9.dev0.tar", last modified: Tue Jan 23 23:44:35 2024, max compression
```

## Comparing `raya-3.7.8.dev0.tar` & `raya-3.7.9.dev0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/setup.cfg
--rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2024-01-22 23:06:31.000000 raya-3.7.8.dev0/setup.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.276999 raya-3.7.8.dev0/src/
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2022-10-07 18:48:43.000000 raya-3.7.8.dev0/src/raya/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       25 2024-01-22 23:06:22.000000 raya-3.7.8.dev0/src/raya/_version.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2119 2024-01-22 23:06:29.000000 raya-3.7.8.dev0/src/raya/application_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      698 2024-01-22 23:06:29.000000 raya-3.7.8.dev0/src/raya/constants.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/controllers/
--rw-rw-r--   0 prod      (1001) prod      (1001)     1552 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      260 2024-01-22 23:06:31.000000 raya-3.7.8.dev0/src/raya/controllers/analytics_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    27599 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/arms_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1562 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/base_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       90 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/base_pseudo_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2690 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/cameras_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      925 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/communication_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2934 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/cv_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1606 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/fleet_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      523 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/grasping_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      924 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/interactions_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1322 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/leds_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1114 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/lidar_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/manipulation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2579 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/motion_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     8381 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/navigation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1922 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/nlp_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      870 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/rgs_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1613 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/sensors_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3666 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/sound_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1368 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/controllers/status_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     9974 2024-01-22 23:06:31.000000 raya-3.7.8.dev0/src/raya/controllers/ui_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       59 2024-01-22 23:06:29.000000 raya-3.7.8.dev0/src/raya/entry_point.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    11328 2024-01-22 23:06:29.000000 raya-3.7.8.dev0/src/raya/enumerations.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    14966 2024-01-09 23:45:58.000000 raya-3.7.8.dev0/src/raya/exceptions.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      279 2024-01-22 23:06:29.000000 raya-3.7.8.dev0/src/raya/exceptions_bases.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     8312 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/exceptions_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2022-12-22 18:51:15.000000 raya-3.7.8.dev0/src/raya/handlers/__init__.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/cv/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2022-12-22 18:51:15.000000 raya-3.7.8.dev0/src/raya/handlers/cv/__init__.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/cv/classifiers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.8.dev0/src/raya/handlers/cv/classifiers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1159 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      802 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/cv/detectors/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.8.dev0/src/raya/handlers/cv/detectors/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1116 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/detectors/detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      312 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/detectors/faces_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      792 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      713 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/cv/estimators/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.8.dev0/src/raya/handlers/cv/estimators/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1127 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/estimators/estimator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      316 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/estimators/hand_estimator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1161 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/model_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/cv/recognizers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.8.dev0/src/raya/handlers/cv/recognizers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      843 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1138 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      807 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      796 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1149 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/handlers/general/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2022-12-28 19:13:50.000000 raya-3.7.8.dev0/src/raya/handlers/general/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      330 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/handlers/general/callback_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/listeners/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2021-10-27 03:02:35.000000 raya-3.7.8.dev0/src/raya/listeners/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       77 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/listeners/lidar_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      160 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/listeners/sensors_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1436 2024-01-22 23:06:29.000000 raya-3.7.8.dev0/src/raya/logger.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2405 2024-01-22 23:06:29.000000 raya-3.7.8.dev0/src/raya/raya_interface.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/skills/
--rw-rw-r--   0 prod      (1001) prod      (1001)      104 2023-10-05 20:17:40.000000 raya-3.7.8.dev0/src/raya/skills/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1023 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/skills/fsm_skill.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2265 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/skills/skill.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      257 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/standalone_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya/tools/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2021-10-30 01:01:46.000000 raya-3.7.8.dev0/src/raya/tools/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      393 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/tools/filesystem.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1919 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/tools/fsm.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      423 2024-01-22 23:06:30.000000 raya-3.7.8.dev0/src/raya/tools/image.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:06:31.280999 raya-3.7.8.dev0/src/raya.egg-info/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2024-01-22 23:06:31.000000 raya-3.7.8.dev0/src/raya.egg-info/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)     2820 2024-01-22 23:06:31.000000 raya-3.7.8.dev0/src/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        1 2024-01-22 23:06:31.000000 raya-3.7.8.dev0/src/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        5 2024-01-22 23:06:31.000000 raya-3.7.8.dev0/src/raya.egg-info/top_level.txt
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.885036 raya-3.7.9.dev0/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2024-01-23 23:44:35.885036 raya-3.7.9.dev0/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2024-01-23 23:44:35.885036 raya-3.7.9.dev0/setup.cfg
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/setup.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2022-10-07 18:48:43.000000 raya-3.7.9.dev0/src/raya/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       25 2024-01-23 23:44:26.000000 raya-3.7.9.dev0/src/raya/_version.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2119 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/application_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      698 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/constants.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/controllers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1552 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      260 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    27599 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1562 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       90 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2690 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      925 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2934 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1606 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      523 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      924 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1322 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1114 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2579 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8381 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1922 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/controllers/nlp_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      870 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/rgs_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1613 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3666 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1368 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/status_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     9974 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       59 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/entry_point.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    11328 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/enumerations.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    14966 2024-01-09 23:45:58.000000 raya-3.7.9.dev0/src/raya/exceptions.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      279 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/exceptions_bases.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8312 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/exceptions_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/handlers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2022-12-22 18:51:15.000000 raya-3.7.9.dev0/src/raya/handlers/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/handlers/cv/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2022-12-22 18:51:15.000000 raya-3.7.9.dev0/src/raya/handlers/cv/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/handlers/cv/classifiers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.9.dev0/src/raya/handlers/cv/classifiers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1159 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      802 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/handlers/cv/detectors/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.9.dev0/src/raya/handlers/cv/detectors/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1116 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/detectors/detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      312 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/detectors/faces_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      792 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      713 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/handlers/cv/estimators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.9.dev0/src/raya/handlers/cv/estimators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1127 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/estimators/estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      316 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/estimators/hand_estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1161 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/model_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/handlers/cv/recognizers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.9.dev0/src/raya/handlers/cv/recognizers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      843 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1138 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-05 14:02:55.000000 raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      807 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      796 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1149 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.885036 raya-3.7.9.dev0/src/raya/handlers/general/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2022-12-28 19:13:50.000000 raya-3.7.9.dev0/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      330 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.885036 raya-3.7.9.dev0/src/raya/listeners/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2021-10-27 03:02:35.000000 raya-3.7.9.dev0/src/raya/listeners/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       77 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      160 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1436 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/logger.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2405 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/raya_interface.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.885036 raya-3.7.9.dev0/src/raya/skills/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      104 2023-10-05 20:17:40.000000 raya-3.7.9.dev0/src/raya/skills/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1023 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/skills/fsm_skill.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2265 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/skills/skill.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      257 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/standalone_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.885036 raya-3.7.9.dev0/src/raya/tools/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2021-10-30 01:01:46.000000 raya-3.7.9.dev0/src/raya/tools/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      393 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/tools/filesystem.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1919 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/tools/fsm.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      423 2024-01-23 23:44:34.000000 raya-3.7.9.dev0/src/raya/tools/image.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:44:35.881036 raya-3.7.9.dev0/src/raya.egg-info/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2820 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        1 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        5 2024-01-23 23:44:35.000000 raya-3.7.9.dev0/src/raya.egg-info/top_level.txt
```

### Comparing `raya-3.7.8.dev0/PKG-INFO` & `raya-3.7.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.7.8.dev0
+Version: 3.7.9.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.7.8.dev0/setup.py` & `raya-3.7.9.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/application_base.py` & `raya-3.7.9.dev0/src/raya/application_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/constants.py` & `raya-3.7.9.dev0/src/raya/constants.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/__init__.py` & `raya-3.7.9.dev0/src/raya/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/arms_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/arms_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/base_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/cameras_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/cameras_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/communication_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/communication_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/cv_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/cv_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/fleet_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/fleet_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/grasping_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/grasping_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/interactions_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/interactions_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/leds_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/leds_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/lidar_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/lidar_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/manipulation_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/manipulation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/motion_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/motion_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/navigation_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/nlp_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/nlp_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/rgs_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/rgs_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/sensors_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/sensors_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/sound_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/sound_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/status_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/status_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/controllers/ui_controller.py` & `raya-3.7.9.dev0/src/raya/controllers/ui_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/enumerations.py` & `raya-3.7.9.dev0/src/raya/enumerations.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/exceptions.py` & `raya-3.7.9.dev0/src/raya/exceptions.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/exceptions_handler.py` & `raya-3.7.9.dev0/src/raya/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/detectors/detector_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/detectors/detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/estimators/estimator_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/estimators/estimator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/model_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/model_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py` & `raya-3.7.9.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/logger.py` & `raya-3.7.9.dev0/src/raya/logger.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/raya_interface.py` & `raya-3.7.9.dev0/src/raya/raya_interface.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/skills/fsm_skill.py` & `raya-3.7.9.dev0/src/raya/skills/fsm_skill.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/skills/skill.py` & `raya-3.7.9.dev0/src/raya/skills/skill.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya/tools/fsm.py` & `raya-3.7.9.dev0/src/raya/tools/fsm.py`

 * *Files identical despite different names*

### Comparing `raya-3.7.8.dev0/src/raya.egg-info/PKG-INFO` & `raya-3.7.9.dev0/src/raya.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.7.8.dev0
+Version: 3.7.9.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.7.8.dev0/src/raya.egg-info/SOURCES.txt` & `raya-3.7.9.dev0/src/raya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

