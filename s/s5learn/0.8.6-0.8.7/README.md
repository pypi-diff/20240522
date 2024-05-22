# Comparing `tmp/s5learn-0.8.6.tar.gz` & `tmp/s5learn-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.8.6.tar", last modified: Wed May 22 17:15:20 2024, max compression
+gzip compressed data, was "s5learn-0.8.7.tar", last modified: Wed May 22 20:20:55 2024, max compression
```

## Comparing `s5learn-0.8.6.tar` & `s5learn-0.8.7.tar`

### file list

```diff
@@ -1,61 +1,72 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 17:15:20.512848 s5learn-0.8.6/
--rw-rw-rw-   0        0        0       54 2024-05-22 17:15:20.504849 s5learn-0.8.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 17:15:20.356508 s5learn-0.8.6/s5learn/
-drwxrwxrwx   0        0        0        0 2024-05-22 17:15:20.377637 s5learn-0.8.6/s5learn/KMeans/
--rw-rw-rw-   0        0        0       30 2024-05-22 17:14:56.000000 s5learn-0.8.6/s5learn/KMeans/__init__.py
--rw-rw-rw-   0        0        0     3567 2024-05-22 17:14:56.000000 s5learn-0.8.6/s5learn/KMeans/kmeans.py
--rw-rw-rw-   0        0        0       28 2024-05-19 23:40:29.000000 s5learn-0.8.6/s5learn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:15:20.393272 s5learn-0.8.6/s5learn/linear_models/
--rw-rw-rw-   0        0        0      518 2024-05-21 22:52:34.000000 s5learn-0.8.6/s5learn/linear_models/__init__.py
--rw-rw-rw-   0        0        0    12290 2024-05-21 03:38:56.000000 s5learn-0.8.6/s5learn/linear_models/cclib.py
--rw-rw-rw-   0        0        0    10713 2024-05-21 03:39:37.000000 s5learn-0.8.6/s5learn/linear_models/dplib.py
--rw-rw-rw-   0        0        0     9282 2024-05-21 03:41:49.000000 s5learn-0.8.6/s5learn/linear_models/fdlib.py
--rw-rw-rw-   0        0        0     9281 2024-05-21 03:42:43.000000 s5learn-0.8.6/s5learn/linear_models/geslib.py
--rw-rw-rw-   0        0        0      910 2024-05-21 03:56:09.000000 s5learn-0.8.6/s5learn/linear_models/ha10lib.py
--rw-rw-rw-   0        0        0     1909 2024-05-21 03:45:49.000000 s5learn-0.8.6/s5learn/linear_models/hblib.py
--rw-rw-rw-   0        0        0     3567 2024-05-21 03:54:13.000000 s5learn-0.8.6/s5learn/linear_models/hpplib.py
--rw-rw-rw-   0        0        0      931 2024-05-21 03:54:13.000000 s5learn-0.8.6/s5learn/linear_models/kafkalib.py
--rw-rw-rw-   0        0        0     1599 2024-05-21 03:56:09.000000 s5learn-0.8.6/s5learn/linear_models/luxlib.py
--rw-rw-rw-   0        0        0     7638 2024-05-21 03:59:30.000000 s5learn-0.8.6/s5learn/linear_models/ofblib.py
--rw-rw-rw-   0        0        0     5879 2024-05-21 04:01:45.000000 s5learn-0.8.6/s5learn/linear_models/pylib.py
--rw-rw-rw-   0        0        0    11238 2024-05-21 04:32:15.000000 s5learn-0.8.6/s5learn/linear_models/sparklib.py
--rw-rw-rw-   0        0        0     2221 2024-05-21 04:32:59.000000 s5learn-0.8.6/s5learn/linear_models/splib.py
--rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8.6/s5learn/main.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:15:20.440139 s5learn-0.8.6/s5learn/models/
--rw-rw-rw-   0        0        0      607 2024-05-21 22:52:34.000000 s5learn-0.8.6/s5learn/models/__init__.py
--rw-rw-rw-   0        0        0      439 2024-05-20 05:13:00.000000 s5learn-0.8.6/s5learn/models/aomalarm.py
--rw-rw-rw-   0        0        0     2834 2024-05-20 05:17:20.000000 s5learn-0.8.6/s5learn/models/aommon.py
--rw-rw-rw-   0        0        0      414 2024-05-20 05:00:54.000000 s5learn-0.8.6/s5learn/models/appscript.py
--rw-rw-rw-   0        0        0      655 2024-05-20 04:59:45.000000 s5learn-0.8.6/s5learn/models/confmysql.py
--rw-rw-rw-   0        0        0      768 2024-05-20 05:09:37.000000 s5learn-0.8.6/s5learn/models/diz.py
--rw-rw-rw-   0        0        0     1338 2024-05-20 05:20:45.000000 s5learn-0.8.6/s5learn/models/dizcon.py
--rw-rw-rw-   0        0        0     8081 2024-05-20 05:21:32.000000 s5learn-0.8.6/s5learn/models/docker.py
--rw-rw-rw-   0        0        0     4632 2024-05-20 05:15:31.000000 s5learn-0.8.6/s5learn/models/dockerfile.py
--rw-rw-rw-   0        0        0      827 2024-05-20 04:57:50.000000 s5learn-0.8.6/s5learn/models/impddm.py
--rw-rw-rw-   0        0        0      690 2024-05-20 05:06:05.000000 s5learn-0.8.6/s5learn/models/logaom.py
--rw-rw-rw-   0        0        0     3381 2024-05-20 05:09:26.000000 s5learn-0.8.6/s5learn/models/micro.py
--rw-rw-rw-   0        0        0     2154 2024-05-20 05:02:05.000000 s5learn-0.8.6/s5learn/models/mysqlcnf.py
--rw-rw-rw-   0        0        0      956 2024-05-20 04:57:04.000000 s5learn-0.8.6/s5learn/models/opcart.py
--rw-rw-rw-   0        0        0      570 2024-05-20 05:04:21.000000 s5learn-0.8.6/s5learn/models/sms.py
--rw-rw-rw-   0        0        0     1832 2024-05-20 04:54:51.000000 s5learn-0.8.6/s5learn/models/wpress.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:15:20.496847 s5learn-0.8.6/s5learn/preprocessing/
--rw-rw-rw-   0        0        0      438 2024-05-21 22:52:34.000000 s5learn-0.8.6/s5learn/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.8.6/s5learn/preprocessing/idp.py
--rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.8.6/s5learn/preprocessing/m5.py
--rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.8.6/s5learn/preprocessing/mnv2.py
--rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.8.6/s5learn/preprocessing/mnv2_dp.py
--rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.8.6/s5learn/preprocessing/mnv2_dv.py
--rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.8.6/s5learn/preprocessing/ms.py
--rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.8.6/s5learn/preprocessing/mv2_train.py
--rw-rw-rw-   0        0        0     3417 2024-05-21 02:49:46.000000 s5learn-0.8.6/s5learn/preprocessing/sp.py
--rw-rw-rw-   0        0        0     7533 2024-05-21 02:52:04.000000 s5learn-0.8.6/s5learn/preprocessing/ss_seqseq.py
--rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.8.6/s5learn/preprocessing/t5.py
--rw-rw-rw-   0        0        0     9982 2024-05-21 02:53:40.000000 s5learn-0.8.6/s5learn/preprocessing/tn.py
--rw-rw-rw-   0        0        0    12019 2024-05-21 02:55:38.000000 s5learn-0.8.6/s5learn/preprocessing/translate.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:15:20.504849 s5learn-0.8.6/s5learn.egg-info/
--rw-rw-rw-   0        0        0       54 2024-05-22 17:15:20.000000 s5learn-0.8.6/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2024-05-22 17:15:20.000000 s5learn-0.8.6/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 17:15:20.000000 s5learn-0.8.6/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 17:15:20.000000 s5learn-0.8.6/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 17:15:20.512848 s5learn-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1819 2024-05-22 17:14:56.000000 s5learn-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.474146 s5learn-0.8.7/
+-rw-rw-rw-   0        0        0       54 2024-05-22 20:20:55.458522 s5learn-0.8.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.317907 s5learn-0.8.7/s5learn/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.317907 s5learn-0.8.7/s5learn/KMeans/
+-rw-rw-rw-   0        0        0       30 2024-05-22 17:14:56.000000 s5learn-0.8.7/s5learn/KMeans/__init__.py
+-rw-rw-rw-   0        0        0     3567 2024-05-22 17:14:56.000000 s5learn-0.8.7/s5learn/KMeans/kmeans.py
+-rw-rw-rw-   0        0        0       28 2024-05-19 23:40:29.000000 s5learn-0.8.7/s5learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.364782 s5learn-0.8.7/s5learn/linear_models/
+-rw-rw-rw-   0        0        0      518 2024-05-21 22:52:34.000000 s5learn-0.8.7/s5learn/linear_models/__init__.py
+-rw-rw-rw-   0        0        0    12290 2024-05-21 03:38:56.000000 s5learn-0.8.7/s5learn/linear_models/cclib.py
+-rw-rw-rw-   0        0        0    10713 2024-05-21 03:39:37.000000 s5learn-0.8.7/s5learn/linear_models/dplib.py
+-rw-rw-rw-   0        0        0     9282 2024-05-21 03:41:49.000000 s5learn-0.8.7/s5learn/linear_models/fdlib.py
+-rw-rw-rw-   0        0        0     9281 2024-05-21 03:42:43.000000 s5learn-0.8.7/s5learn/linear_models/geslib.py
+-rw-rw-rw-   0        0        0      910 2024-05-21 03:56:09.000000 s5learn-0.8.7/s5learn/linear_models/ha10lib.py
+-rw-rw-rw-   0        0        0     1909 2024-05-21 03:45:49.000000 s5learn-0.8.7/s5learn/linear_models/hblib.py
+-rw-rw-rw-   0        0        0     3567 2024-05-21 03:54:13.000000 s5learn-0.8.7/s5learn/linear_models/hpplib.py
+-rw-rw-rw-   0        0        0      931 2024-05-21 03:54:13.000000 s5learn-0.8.7/s5learn/linear_models/kafkalib.py
+-rw-rw-rw-   0        0        0     1599 2024-05-21 03:56:09.000000 s5learn-0.8.7/s5learn/linear_models/luxlib.py
+-rw-rw-rw-   0        0        0     7638 2024-05-21 03:59:30.000000 s5learn-0.8.7/s5learn/linear_models/ofblib.py
+-rw-rw-rw-   0        0        0     5879 2024-05-21 04:01:45.000000 s5learn-0.8.7/s5learn/linear_models/pylib.py
+-rw-rw-rw-   0        0        0    11238 2024-05-21 04:32:15.000000 s5learn-0.8.7/s5learn/linear_models/sparklib.py
+-rw-rw-rw-   0        0        0     2221 2024-05-21 04:32:59.000000 s5learn-0.8.7/s5learn/linear_models/splib.py
+-rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8.7/s5learn/main.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.380402 s5learn-0.8.7/s5learn/model_selection/
+-rw-rw-rw-   0        0        0      332 2024-05-22 20:20:26.000000 s5learn-0.8.7/s5learn/model_selection/__init__.py
+-rw-rw-rw-   0        0        0      849 2024-05-22 18:21:40.000000 s5learn-0.8.7/s5learn/model_selection/a_1_2.py
+-rw-rw-rw-   0        0        0      273 2024-05-22 18:23:53.000000 s5learn-0.8.7/s5learn/model_selection/a_1_3.py
+-rw-rw-rw-   0        0        0     1247 2024-05-22 18:30:00.000000 s5learn-0.8.7/s5learn/model_selection/a_2_1.py
+-rw-rw-rw-   0        0        0     1748 2024-05-22 18:36:13.000000 s5learn-0.8.7/s5learn/model_selection/a_2_2.py
+-rw-rw-rw-   0        0        0     5267 2024-05-22 18:37:29.000000 s5learn-0.8.7/s5learn/model_selection/a_2_3.py
+-rw-rw-rw-   0        0        0      798 2024-05-22 18:44:46.000000 s5learn-0.8.7/s5learn/model_selection/a_2_4.py
+-rw-rw-rw-   0        0        0      261 2024-05-22 18:39:49.000000 s5learn-0.8.7/s5learn/model_selection/a_3_1_2.py
+-rw-rw-rw-   0        0        0      910 2024-05-22 18:26:16.000000 s5learn-0.8.7/s5learn/model_selection/ab_1_4.py
+-rw-rw-rw-   0        0        0     2024 2024-05-22 20:20:26.000000 s5learn-0.8.7/s5learn/model_selection/tn2.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.411651 s5learn-0.8.7/s5learn/models/
+-rw-rw-rw-   0        0        0      603 2024-05-22 20:20:26.000000 s5learn-0.8.7/s5learn/models/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-05-20 05:13:00.000000 s5learn-0.8.7/s5learn/models/aomalarm.py
+-rw-rw-rw-   0        0        0     2834 2024-05-20 05:17:20.000000 s5learn-0.8.7/s5learn/models/aommon.py
+-rw-rw-rw-   0        0        0      414 2024-05-20 05:00:54.000000 s5learn-0.8.7/s5learn/models/appscript.py
+-rw-rw-rw-   0        0        0      655 2024-05-20 04:59:45.000000 s5learn-0.8.7/s5learn/models/confmysql.py
+-rw-rw-rw-   0        0        0      768 2024-05-20 05:09:37.000000 s5learn-0.8.7/s5learn/models/diz.py
+-rw-rw-rw-   0        0        0     1338 2024-05-20 05:20:45.000000 s5learn-0.8.7/s5learn/models/dizcon.py
+-rw-rw-rw-   0        0        0     8081 2024-05-20 05:21:32.000000 s5learn-0.8.7/s5learn/models/docker.py
+-rw-rw-rw-   0        0        0     4632 2024-05-20 05:15:31.000000 s5learn-0.8.7/s5learn/models/dockerfile.py
+-rw-rw-rw-   0        0        0      827 2024-05-20 04:57:50.000000 s5learn-0.8.7/s5learn/models/impddm.py
+-rw-rw-rw-   0        0        0      690 2024-05-20 05:06:05.000000 s5learn-0.8.7/s5learn/models/logaom.py
+-rw-rw-rw-   0        0        0     3381 2024-05-20 05:09:26.000000 s5learn-0.8.7/s5learn/models/micro.py
+-rw-rw-rw-   0        0        0     2154 2024-05-20 05:02:05.000000 s5learn-0.8.7/s5learn/models/mysqlcnf.py
+-rw-rw-rw-   0        0        0      956 2024-05-20 04:57:04.000000 s5learn-0.8.7/s5learn/models/opcart.py
+-rw-rw-rw-   0        0        0      570 2024-05-20 05:04:21.000000 s5learn-0.8.7/s5learn/models/sms.py
+-rw-rw-rw-   0        0        0     1832 2024-05-20 04:54:51.000000 s5learn-0.8.7/s5learn/models/wpress.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.458522 s5learn-0.8.7/s5learn/preprocessing/
+-rw-rw-rw-   0        0        0      434 2024-05-22 20:20:26.000000 s5learn-0.8.7/s5learn/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.8.7/s5learn/preprocessing/idp.py
+-rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.8.7/s5learn/preprocessing/m5.py
+-rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.8.7/s5learn/preprocessing/mnv2.py
+-rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.8.7/s5learn/preprocessing/mnv2_dp.py
+-rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.8.7/s5learn/preprocessing/mnv2_dv.py
+-rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.8.7/s5learn/preprocessing/ms.py
+-rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.8.7/s5learn/preprocessing/mv2_train.py
+-rw-rw-rw-   0        0        0     3417 2024-05-21 02:49:46.000000 s5learn-0.8.7/s5learn/preprocessing/sp.py
+-rw-rw-rw-   0        0        0     7533 2024-05-21 02:52:04.000000 s5learn-0.8.7/s5learn/preprocessing/ss_seqseq.py
+-rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.8.7/s5learn/preprocessing/t5.py
+-rw-rw-rw-   0        0        0     9982 2024-05-21 02:53:40.000000 s5learn-0.8.7/s5learn/preprocessing/tn.py
+-rw-rw-rw-   0        0        0    12019 2024-05-21 02:55:38.000000 s5learn-0.8.7/s5learn/preprocessing/translate.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:20:55.458522 s5learn-0.8.7/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-05-22 20:20:55.000000 s5learn-0.8.7/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1816 2024-05-22 20:20:55.000000 s5learn-0.8.7/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:20:55.000000 s5learn-0.8.7/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 20:20:55.000000 s5learn-0.8.7/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:20:55.474146 s5learn-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2024-05-22 20:20:26.000000 s5learn-0.8.7/setup.py
```

### Comparing `s5learn-0.8.6/s5learn/KMeans/kmeans.py` & `s5learn-0.8.7/s5learn/KMeans/kmeans.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/__init__.py` & `s5learn-0.8.7/s5learn/linear_models/__init__.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/cclib.py` & `s5learn-0.8.7/s5learn/linear_models/cclib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/dplib.py` & `s5learn-0.8.7/s5learn/linear_models/dplib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/fdlib.py` & `s5learn-0.8.7/s5learn/linear_models/fdlib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/geslib.py` & `s5learn-0.8.7/s5learn/linear_models/geslib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/ha10lib.py` & `s5learn-0.8.7/s5learn/linear_models/ha10lib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/hblib.py` & `s5learn-0.8.7/s5learn/linear_models/hblib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/hpplib.py` & `s5learn-0.8.7/s5learn/linear_models/hpplib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/kafkalib.py` & `s5learn-0.8.7/s5learn/linear_models/kafkalib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/luxlib.py` & `s5learn-0.8.7/s5learn/linear_models/luxlib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/ofblib.py` & `s5learn-0.8.7/s5learn/linear_models/ofblib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/pylib.py` & `s5learn-0.8.7/s5learn/linear_models/pylib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/sparklib.py` & `s5learn-0.8.7/s5learn/linear_models/sparklib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/linear_models/splib.py` & `s5learn-0.8.7/s5learn/linear_models/splib.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/__init__.py` & `s5learn-0.8.7/s5learn/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,8 @@
 from .logaom import logaom
 from .micro import micro
 from .mysqlcnf import mysqlcnf
 from .opcart import opcart
 from .sms import sms
 from .wpress import wpress
 
-
-
 __all__ = ['aomalarm', 'aommon', 'appscript', 'confmysql', 'diz', 'dizcon', 'docker', 'dockerfile', 'impddm', 'logaom', 'micro', 'mysqlcnf', 'opcart', 'sms', 'wpress']
```

### Comparing `s5learn-0.8.6/s5learn/models/aommon.py` & `s5learn-0.8.7/s5learn/models/aommon.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/confmysql.py` & `s5learn-0.8.7/s5learn/models/confmysql.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/diz.py` & `s5learn-0.8.7/s5learn/models/diz.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/dizcon.py` & `s5learn-0.8.7/s5learn/models/dizcon.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/docker.py` & `s5learn-0.8.7/s5learn/models/docker.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/dockerfile.py` & `s5learn-0.8.7/s5learn/models/dockerfile.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/impddm.py` & `s5learn-0.8.7/s5learn/models/impddm.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/logaom.py` & `s5learn-0.8.7/s5learn/models/logaom.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/micro.py` & `s5learn-0.8.7/s5learn/models/micro.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/mysqlcnf.py` & `s5learn-0.8.7/s5learn/models/mysqlcnf.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/opcart.py` & `s5learn-0.8.7/s5learn/models/opcart.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/sms.py` & `s5learn-0.8.7/s5learn/models/sms.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/models/wpress.py` & `s5learn-0.8.7/s5learn/models/wpress.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/idp.py` & `s5learn-0.8.7/s5learn/preprocessing/idp.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/m5.py` & `s5learn-0.8.7/s5learn/preprocessing/m5.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/mnv2.py` & `s5learn-0.8.7/s5learn/preprocessing/mnv2.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/mnv2_dp.py` & `s5learn-0.8.7/s5learn/preprocessing/mnv2_dp.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/mnv2_dv.py` & `s5learn-0.8.7/s5learn/preprocessing/mnv2_dv.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/ms.py` & `s5learn-0.8.7/s5learn/preprocessing/ms.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/mv2_train.py` & `s5learn-0.8.7/s5learn/preprocessing/mv2_train.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/sp.py` & `s5learn-0.8.7/s5learn/preprocessing/sp.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/ss_seqseq.py` & `s5learn-0.8.7/s5learn/preprocessing/ss_seqseq.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/t5.py` & `s5learn-0.8.7/s5learn/preprocessing/t5.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/tn.py` & `s5learn-0.8.7/s5learn/preprocessing/tn.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/s5learn/preprocessing/translate.py` & `s5learn-0.8.7/s5learn/preprocessing/translate.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.6/setup.py` & `s5learn-0.8.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.8.6',
+    version='0.8.7',
     packages=find_packages(),
     package_data={'': ['data/*.txt']},
 )
 
 
 
 # import setuptools
```

