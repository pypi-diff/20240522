# Comparing `tmp/lesscode_charts-0.0.8.tar.gz` & `tmp/lesscode_charts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_charts-0.0.8.tar", last modified: Mon Sep 11 03:25:01 2023, max compression
+gzip compressed data, was "dist/lesscode_charts-0.0.9.tar", last modified: Tue Sep 12 09:13:54 2023, max compression
```

## Comparing `lesscode_charts-0.0.8.tar` & `lesscode_charts-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.8/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.8/lesscode_charts/__init__.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts/utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.8/lesscode_charts/utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.8/lesscode_charts/utils/common_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts/v1/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.8/lesscode_charts/v1/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.8/lesscode_charts/v1/forest_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3599 2023-09-11 03:24:54.000000 lesscode_charts-0.0.8/lesscode_charts/v1/histogram_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.8/lesscode_charts/v1/k_line_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1444 2023-07-04 08:44:48.000000 lesscode_charts-0.0.8/lesscode_charts/v1/pie_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1277 2023-09-11 03:24:54.000000 lesscode_charts-0.0.8/lesscode_charts/v1/pyramid_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      919 2023-09-11 03:24:54.000000 lesscode_charts-0.0.8/lesscode_charts/v1/radar_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 11:03:04.000000 lesscode_charts-0.0.8/lesscode_charts/v1/sankey_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3125 2023-07-27 02:32:26.000000 lesscode_charts-0.0.8/lesscode_charts/v1/table_chart.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-09-11 03:24:54.000000 lesscode_charts-0.0.8/lesscode_charts/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      611 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/lesscode_charts.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-09-11 03:25:01.000000 lesscode_charts-0.0.8/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.8/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-12 09:13:54.000000 lesscode_charts-0.0.9/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-09-12 09:13:54.000000 lesscode_charts-0.0.9/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.9/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-12 09:13:54.000000 lesscode_charts-0.0.9/lesscode_charts/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.9/lesscode_charts/__init__.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-12 09:13:54.000000 lesscode_charts-0.0.9/lesscode_charts/utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.9/lesscode_charts/utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.9/lesscode_charts/utils/common_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-12 09:13:54.000000 lesscode_charts-0.0.9/lesscode_charts/v1/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.9/lesscode_charts/v1/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.9/lesscode_charts/v1/forest_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3599 2023-09-11 03:24:54.000000 lesscode_charts-0.0.9/lesscode_charts/v1/histogram_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.9/lesscode_charts/v1/k_line_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1516 2023-09-12 09:10:13.000000 lesscode_charts-0.0.9/lesscode_charts/v1/pie_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1277 2023-09-11 03:24:54.000000 lesscode_charts-0.0.9/lesscode_charts/v1/pyramid_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      919 2023-09-11 03:24:54.000000 lesscode_charts-0.0.9/lesscode_charts/v1/radar_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 11:03:04.000000 lesscode_charts-0.0.9/lesscode_charts/v1/sankey_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3125 2023-07-27 02:32:26.000000 lesscode_charts-0.0.9/lesscode_charts/v1/table_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-09-12 09:13:47.000000 lesscode_charts-0.0.9/lesscode_charts/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-09-12 09:13:54.000000 lesscode_charts-0.0.9/lesscode_charts.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-09-12 09:13:53.000000 lesscode_charts-0.0.9/lesscode_charts.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      611 2023-09-12 09:13:53.000000 lesscode_charts-0.0.9/lesscode_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-09-12 09:13:53.000000 lesscode_charts-0.0.9/lesscode_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-09-12 09:13:53.000000 lesscode_charts-0.0.9/lesscode_charts.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-09-12 09:13:54.000000 lesscode_charts-0.0.9/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.9/setup.py
```

### Comparing `lesscode_charts-0.0.8/lesscode_charts/utils/common_utils.py` & `lesscode_charts-0.0.9/lesscode_charts/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/forest_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/forest_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/histogram_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/histogram_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/k_line_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/k_line_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/pie_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/pie_chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         @return:
         """
         new_data = dict()
         if data_key is not None:
             for key, value in data.items():
                 if isinstance(value, dict):
                     new_data.update({key: value.get(data_key)})
+                else:
+                    new_data.update({key: value})
         else:
             new_data = data
         if total is None:
             total = sum([_ for _ in new_data.values()])
         if total == 0:
             total = 1
         result = {
```

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/pyramid_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/pyramid_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/radar_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/radar_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/sankey_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/sankey_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts/v1/table_chart.py` & `lesscode_charts-0.0.9/lesscode_charts/v1/table_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/lesscode_charts.egg-info/SOURCES.txt` & `lesscode_charts-0.0.9/lesscode_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.8/setup.py` & `lesscode_charts-0.0.9/setup.py`

 * *Files identical despite different names*

