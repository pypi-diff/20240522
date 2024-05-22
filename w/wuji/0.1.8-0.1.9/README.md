# Comparing `tmp/wuji-0.1.8.tar.gz` & `tmp/wuji-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wuji-0.1.8.tar", last modified: Fri Nov  3 08:35:11 2023, max compression
+gzip compressed data, was "wuji-0.1.9.tar", last modified: Tue Nov  7 08:26:46 2023, max compression
```

## Comparing `wuji-0.1.8.tar` & `wuji-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.370942 wuji-0.1.8/
--rw-r--r--   0 cxs        (502) staff       (20)      110 2023-11-03 08:35:11.370774 wuji-0.1.8/PKG-INFO
--rw-r--r--   0 cxs        (502) staff       (20)       38 2023-11-03 08:35:11.371000 wuji-0.1.8/setup.cfg
--rw-r--r--   0 cxs        (502) staff       (20)      368 2023-11-03 08:35:06.000000 wuji-0.1.8/setup.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.365937 wuji-0.1.8/wuji/
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.366930 wuji-0.1.8/wuji/Evaluator/
--rw-r--r--   0 cxs        (502) staff       (20)     1763 2023-09-22 07:40:32.000000 wuji-0.1.8/wuji/Evaluator/Classification.py
--rw-r--r--   0 cxs        (502) staff       (20)     3305 2023-10-07 02:14:10.000000 wuji-0.1.8/wuji/Evaluator/EventDetector.py
--rw-r--r--   0 cxs        (502) staff       (20)     2910 2023-09-27 07:30:26.000000 wuji-0.1.8/wuji/Evaluator/NightlySleepMetrics.py
--rw-r--r--   0 cxs        (502) staff       (20)      168 2023-09-21 13:47:55.000000 wuji-0.1.8/wuji/Evaluator/__init__.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.367168 wuji-0.1.8/wuji/Reader/
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.367645 wuji-0.1.8/wuji/Reader/Annotation/
--rw-r--r--   0 cxs        (502) staff       (20)     4083 2023-09-25 09:55:52.000000 wuji-0.1.8/wuji/Reader/Annotation/Base.py
--rw-r--r--   0 cxs        (502) staff       (20)     2079 2023-09-14 09:37:20.000000 wuji-0.1.8/wuji/Reader/Annotation/NSRR.py
--rw-r--r--   0 cxs        (502) staff       (20)     3383 2023-10-09 13:35:02.000000 wuji-0.1.8/wuji/Reader/Annotation/Philips.py
--rw-r--r--   0 cxs        (502) staff       (20)      168 2023-08-17 08:48:55.000000 wuji-0.1.8/wuji/Reader/Annotation/__init__.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.368137 wuji-0.1.8/wuji/Reader/EDF/
--rw-r--r--   0 cxs        (502) staff       (20)     3442 2023-11-03 08:18:38.000000 wuji-0.1.8/wuji/Reader/EDF/Base.py
--rw-r--r--   0 cxs        (502) staff       (20)      555 2023-09-14 11:36:25.000000 wuji-0.1.8/wuji/Reader/EDF/NSRR.py
--rw-r--r--   0 cxs        (502) staff       (20)      305 2023-09-14 11:36:25.000000 wuji-0.1.8/wuji/Reader/EDF/Philips.py
--rw-r--r--   0 cxs        (502) staff       (20)      168 2023-08-17 08:48:55.000000 wuji-0.1.8/wuji/Reader/EDF/__init__.py
--rw-r--r--   0 cxs        (502) staff       (20)      354 2023-11-03 07:26:04.000000 wuji-0.1.8/wuji/Reader/__init__.py
--rw-r--r--   0 cxs        (502) staff       (20)     1522 2023-09-28 06:29:37.000000 wuji-0.1.8/wuji/Reader/utils.py
--rw-r--r--   0 cxs        (502) staff       (20)      168 2023-09-14 09:32:00.000000 wuji-0.1.8/wuji/__init__.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.368746 wuji-0.1.8/wuji/examples/
--rw-r--r--   0 cxs        (502) staff       (20)      165 2023-09-27 07:26:12.000000 wuji-0.1.8/wuji/examples/__init__.py
--rw-r--r--   0 cxs        (502) staff       (20)      920 2023-09-22 07:40:53.000000 wuji-0.1.8/wuji/examples/eval_classifier.py
--rw-r--r--   0 cxs        (502) staff       (20)      977 2023-10-31 08:09:31.000000 wuji-0.1.8/wuji/examples/eval_event_detector.py
--rw-r--r--   0 cxs        (502) staff       (20)      581 2023-09-27 07:30:43.000000 wuji-0.1.8/wuji/examples/eval_nightly_sleep_metrics.py
--rw-r--r--   0 cxs        (502) staff       (20)     1272 2023-09-25 06:46:28.000000 wuji-0.1.8/wuji/examples/read_edf_of_Philips.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.369669 wuji-0.1.8/wuji/sed_eval/
--rw-r--r--   0 cxs        (502) staff       (20)      251 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/__init__.py
--rw-r--r--   0 cxs        (502) staff       (20)    24771 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/audio_tag.py
--rw-r--r--   0 cxs        (502) staff       (20)     4249 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/io.py
--rw-r--r--   0 cxs        (502) staff       (20)     8597 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/metric.py
--rw-r--r--   0 cxs        (502) staff       (20)    14803 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/scene.py
--rw-r--r--   0 cxs        (502) staff       (20)    66260 2023-09-26 12:49:48.000000 wuji-0.1.8/wuji/sed_eval/sound_event.py
--rw-r--r--   0 cxs        (502) staff       (20)     1562 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/test.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.370382 wuji-0.1.8/wuji/sed_eval/util/
--rw-r--r--   0 cxs        (502) staff       (20)     1058 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/util/__init__.py
--rw-r--r--   0 cxs        (502) staff       (20)     3009 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/util/event_list.py
--rw-r--r--   0 cxs        (502) staff       (20)     3690 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/util/event_matching.py
--rw-r--r--   0 cxs        (502) staff       (20)     3900 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/util/event_roll.py
--rw-r--r--   0 cxs        (502) staff       (20)      766 2022-11-16 08:20:33.000000 wuji-0.1.8/wuji/sed_eval/util/scene_list.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.370550 wuji-0.1.8/wuji/utils/
--rw-r--r--   0 cxs        (502) staff       (20)      168 2023-09-14 09:34:49.000000 wuji-0.1.8/wuji/utils/__init__.py
-drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-03 08:35:11.366439 wuji-0.1.8/wuji.egg-info/
--rw-r--r--   0 cxs        (502) staff       (20)      110 2023-11-03 08:35:11.000000 wuji-0.1.8/wuji.egg-info/PKG-INFO
--rw-r--r--   0 cxs        (502) staff       (20)     1084 2023-11-03 08:35:11.000000 wuji-0.1.8/wuji.egg-info/SOURCES.txt
--rw-r--r--   0 cxs        (502) staff       (20)        1 2023-11-03 08:35:11.000000 wuji-0.1.8/wuji.egg-info/dependency_links.txt
--rw-r--r--   0 cxs        (502) staff       (20)        5 2023-11-03 08:35:11.000000 wuji-0.1.8/wuji.egg-info/top_level.txt
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.593945 wuji-0.1.9/
+-rw-r--r--   0 cxs        (502) staff       (20)      110 2023-11-07 08:26:46.593735 wuji-0.1.9/PKG-INFO
+-rw-r--r--   0 cxs        (502) staff       (20)       38 2023-11-07 08:26:46.594012 wuji-0.1.9/setup.cfg
+-rw-r--r--   0 cxs        (502) staff       (20)      368 2023-11-07 08:26:40.000000 wuji-0.1.9/setup.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.586207 wuji-0.1.9/wuji/
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.587602 wuji-0.1.9/wuji/Evaluator/
+-rw-r--r--   0 cxs        (502) staff       (20)     1763 2023-09-22 07:40:32.000000 wuji-0.1.9/wuji/Evaluator/Classification.py
+-rw-r--r--   0 cxs        (502) staff       (20)     3305 2023-10-07 02:14:10.000000 wuji-0.1.9/wuji/Evaluator/EventDetector.py
+-rw-r--r--   0 cxs        (502) staff       (20)     2910 2023-09-27 07:30:26.000000 wuji-0.1.9/wuji/Evaluator/NightlySleepMetrics.py
+-rw-r--r--   0 cxs        (502) staff       (20)      168 2023-09-21 13:47:55.000000 wuji-0.1.9/wuji/Evaluator/__init__.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.587863 wuji-0.1.9/wuji/Reader/
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.588714 wuji-0.1.9/wuji/Reader/Annotation/
+-rw-r--r--   0 cxs        (502) staff       (20)     4083 2023-09-25 09:55:52.000000 wuji-0.1.9/wuji/Reader/Annotation/Base.py
+-rw-r--r--   0 cxs        (502) staff       (20)     2079 2023-09-14 09:37:20.000000 wuji-0.1.9/wuji/Reader/Annotation/NSRR.py
+-rw-r--r--   0 cxs        (502) staff       (20)     3383 2023-10-09 13:35:02.000000 wuji-0.1.9/wuji/Reader/Annotation/Philips.py
+-rw-r--r--   0 cxs        (502) staff       (20)      168 2023-08-17 08:48:55.000000 wuji-0.1.9/wuji/Reader/Annotation/__init__.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.589435 wuji-0.1.9/wuji/Reader/EDF/
+-rw-r--r--   0 cxs        (502) staff       (20)     3442 2023-11-03 08:18:38.000000 wuji-0.1.9/wuji/Reader/EDF/Base.py
+-rw-r--r--   0 cxs        (502) staff       (20)      555 2023-09-14 11:36:25.000000 wuji-0.1.9/wuji/Reader/EDF/NSRR.py
+-rw-r--r--   0 cxs        (502) staff       (20)      305 2023-09-14 11:36:25.000000 wuji-0.1.9/wuji/Reader/EDF/Philips.py
+-rw-r--r--   0 cxs        (502) staff       (20)      168 2023-08-17 08:48:55.000000 wuji-0.1.9/wuji/Reader/EDF/__init__.py
+-rw-r--r--   0 cxs        (502) staff       (20)      354 2023-11-03 07:26:04.000000 wuji-0.1.9/wuji/Reader/__init__.py
+-rw-r--r--   0 cxs        (502) staff       (20)     1522 2023-09-28 06:29:37.000000 wuji-0.1.9/wuji/Reader/utils.py
+-rw-r--r--   0 cxs        (502) staff       (20)      168 2023-09-14 09:32:00.000000 wuji-0.1.9/wuji/__init__.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.590371 wuji-0.1.9/wuji/examples/
+-rw-r--r--   0 cxs        (502) staff       (20)      165 2023-09-27 07:26:12.000000 wuji-0.1.9/wuji/examples/__init__.py
+-rw-r--r--   0 cxs        (502) staff       (20)      920 2023-09-22 07:40:53.000000 wuji-0.1.9/wuji/examples/eval_classifier.py
+-rw-r--r--   0 cxs        (502) staff       (20)      977 2023-10-31 08:09:31.000000 wuji-0.1.9/wuji/examples/eval_event_detector.py
+-rw-r--r--   0 cxs        (502) staff       (20)      581 2023-09-27 07:30:43.000000 wuji-0.1.9/wuji/examples/eval_nightly_sleep_metrics.py
+-rw-r--r--   0 cxs        (502) staff       (20)     1272 2023-09-25 06:46:28.000000 wuji-0.1.9/wuji/examples/read_edf_of_Philips.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.591976 wuji-0.1.9/wuji/sed_eval/
+-rw-r--r--   0 cxs        (502) staff       (20)      251 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/__init__.py
+-rw-r--r--   0 cxs        (502) staff       (20)    24771 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/audio_tag.py
+-rw-r--r--   0 cxs        (502) staff       (20)     4249 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/io.py
+-rw-r--r--   0 cxs        (502) staff       (20)     8597 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/metric.py
+-rw-r--r--   0 cxs        (502) staff       (20)    14803 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/scene.py
+-rw-r--r--   0 cxs        (502) staff       (20)    66260 2023-09-26 12:49:48.000000 wuji-0.1.9/wuji/sed_eval/sound_event.py
+-rw-r--r--   0 cxs        (502) staff       (20)     1562 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/test.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.592997 wuji-0.1.9/wuji/sed_eval/util/
+-rw-r--r--   0 cxs        (502) staff       (20)     1058 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/util/__init__.py
+-rw-r--r--   0 cxs        (502) staff       (20)     3009 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/util/event_list.py
+-rw-r--r--   0 cxs        (502) staff       (20)     3690 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/util/event_matching.py
+-rw-r--r--   0 cxs        (502) staff       (20)     3900 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/util/event_roll.py
+-rw-r--r--   0 cxs        (502) staff       (20)      766 2022-11-16 08:20:33.000000 wuji-0.1.9/wuji/sed_eval/util/scene_list.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.593309 wuji-0.1.9/wuji/tools/
+-rw-r--r--   0 cxs        (502) staff       (20)      168 2023-11-07 08:26:02.000000 wuji-0.1.9/wuji/tools/__init__.py
+-rw-r--r--   0 cxs        (502) staff       (20)     1768 2023-11-07 08:26:02.000000 wuji-0.1.9/wuji/tools/cut_edf.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.593455 wuji-0.1.9/wuji/utils/
+-rw-r--r--   0 cxs        (502) staff       (20)      168 2023-09-14 09:34:49.000000 wuji-0.1.9/wuji/utils/__init__.py
+drwxr-xr-x   0 cxs        (502) staff       (20)        0 2023-11-07 08:26:46.586942 wuji-0.1.9/wuji.egg-info/
+-rw-r--r--   0 cxs        (502) staff       (20)      110 2023-11-07 08:26:46.000000 wuji-0.1.9/wuji.egg-info/PKG-INFO
+-rw-r--r--   0 cxs        (502) staff       (20)     1129 2023-11-07 08:26:46.000000 wuji-0.1.9/wuji.egg-info/SOURCES.txt
+-rw-r--r--   0 cxs        (502) staff       (20)        1 2023-11-07 08:26:46.000000 wuji-0.1.9/wuji.egg-info/dependency_links.txt
+-rw-r--r--   0 cxs        (502) staff       (20)        5 2023-11-07 08:26:46.000000 wuji-0.1.9/wuji.egg-info/top_level.txt
```

### Comparing `wuji-0.1.8/wuji/Evaluator/Classification.py` & `wuji-0.1.9/wuji/Evaluator/Classification.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Evaluator/EventDetector.py` & `wuji-0.1.9/wuji/Evaluator/EventDetector.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Evaluator/NightlySleepMetrics.py` & `wuji-0.1.9/wuji/Evaluator/NightlySleepMetrics.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Reader/Annotation/Base.py` & `wuji-0.1.9/wuji/Reader/Annotation/Base.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Reader/Annotation/NSRR.py` & `wuji-0.1.9/wuji/Reader/Annotation/NSRR.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Reader/Annotation/Philips.py` & `wuji-0.1.9/wuji/Reader/Annotation/Philips.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Reader/EDF/Base.py` & `wuji-0.1.9/wuji/Reader/EDF/Base.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Reader/EDF/NSRR.py` & `wuji-0.1.9/wuji/Reader/EDF/NSRR.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/Reader/utils.py` & `wuji-0.1.9/wuji/Reader/utils.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/examples/eval_classifier.py` & `wuji-0.1.9/wuji/examples/eval_classifier.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/examples/eval_event_detector.py` & `wuji-0.1.9/wuji/examples/eval_event_detector.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/examples/eval_nightly_sleep_metrics.py` & `wuji-0.1.9/wuji/examples/eval_nightly_sleep_metrics.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/examples/read_edf_of_Philips.py` & `wuji-0.1.9/wuji/examples/read_edf_of_Philips.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/audio_tag.py` & `wuji-0.1.9/wuji/sed_eval/audio_tag.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/io.py` & `wuji-0.1.9/wuji/sed_eval/io.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/metric.py` & `wuji-0.1.9/wuji/sed_eval/metric.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/scene.py` & `wuji-0.1.9/wuji/sed_eval/scene.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/sound_event.py` & `wuji-0.1.9/wuji/sed_eval/sound_event.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/test.py` & `wuji-0.1.9/wuji/sed_eval/test.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/util/__init__.py` & `wuji-0.1.9/wuji/sed_eval/util/__init__.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/util/event_list.py` & `wuji-0.1.9/wuji/sed_eval/util/event_list.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/util/event_matching.py` & `wuji-0.1.9/wuji/sed_eval/util/event_matching.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/util/event_roll.py` & `wuji-0.1.9/wuji/sed_eval/util/event_roll.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji/sed_eval/util/scene_list.py` & `wuji-0.1.9/wuji/sed_eval/util/scene_list.py`

 * *Files identical despite different names*

### Comparing `wuji-0.1.8/wuji.egg-info/SOURCES.txt` & `wuji-0.1.9/wuji.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 wuji/sed_eval/sound_event.py
 wuji/sed_eval/test.py
 wuji/sed_eval/util/__init__.py
 wuji/sed_eval/util/event_list.py
 wuji/sed_eval/util/event_matching.py
 wuji/sed_eval/util/event_roll.py
 wuji/sed_eval/util/scene_list.py
+wuji/tools/__init__.py
+wuji/tools/cut_edf.py
 wuji/utils/__init__.py
```

