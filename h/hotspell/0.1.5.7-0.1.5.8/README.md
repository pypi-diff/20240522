# Comparing `tmp/hotspell-0.1.5.7.tar.gz` & `tmp/hotspell-0.1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotspell-0.1.5.7.tar", last modified: Fri Nov  3 13:14:15 2023, max compression
+gzip compressed data, was "hotspell-0.1.5.8.tar", last modified: Wed May 22 06:21:14 2024, max compression
```

## Comparing `hotspell-0.1.5.7.tar` & `hotspell-0.1.5.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-11-03 13:14:15.390142 hotspell-0.1.5.7/
--rw-r--r--   0 ilias     (1000) ilias     (1000)     1557 2021-05-13 12:57:40.000000 hotspell-0.1.5.7/LICENSE
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     2612 2023-11-03 13:14:15.390142 hotspell-0.1.5.7/PKG-INFO
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     2362 2021-09-24 15:19:25.000000 hotspell-0.1.5.7/README.rst
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-11-03 13:14:15.390142 hotspell-0.1.5.7/hotspell/
--rw-rw-r--   0 ilias     (1000) ilias     (1000)       64 2021-08-13 06:22:04.000000 hotspell-0.1.5.7/hotspell/__init__.py
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-11-03 13:14:15.390142 hotspell-0.1.5.7/hotspell/datasets/
--rw-rw-r--   0 ilias     (1000) ilias     (1000)    49328 2022-01-30 14:38:16.000000 hotspell-0.1.5.7/hotspell/datasets/daily_windows_with_length_15.pickle
--rw-rw-r--   0 ilias     (1000) ilias     (1000)    14192 2022-01-30 14:38:16.000000 hotspell-0.1.5.7/hotspell/datasets/daily_windows_with_length_3.pickle
--rw-rw-r--   0 ilias     (1000) ilias     (1000)    11837 2023-11-03 11:06:08.000000 hotspell-0.1.5.7/hotspell/heatwaves.py
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     5692 2022-10-22 18:30:31.000000 hotspell-0.1.5.7/hotspell/indices.py
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     3291 2022-10-22 18:20:02.000000 hotspell-0.1.5.7/hotspell/metrics.py
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     2901 2023-11-03 11:17:29.000000 hotspell-0.1.5.7/hotspell/utils.py
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-11-03 13:14:15.390142 hotspell-0.1.5.7/hotspell.egg-info/
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     2612 2023-11-03 13:14:15.000000 hotspell-0.1.5.7/hotspell.egg-info/PKG-INFO
--rw-rw-r--   0 ilias     (1000) ilias     (1000)      418 2023-11-03 13:14:15.000000 hotspell-0.1.5.7/hotspell.egg-info/SOURCES.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)        1 2023-11-03 13:14:15.000000 hotspell-0.1.5.7/hotspell.egg-info/dependency_links.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)       13 2023-11-03 13:14:15.000000 hotspell-0.1.5.7/hotspell.egg-info/requires.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)        9 2023-11-03 13:14:15.000000 hotspell-0.1.5.7/hotspell.egg-info/top_level.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)       38 2023-11-03 13:14:15.390142 hotspell-0.1.5.7/setup.cfg
--rw-rw-r--   0 ilias     (1000) ilias     (1000)      625 2023-11-03 13:14:00.000000 hotspell-0.1.5.7/setup.py
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-11-03 13:14:15.390142 hotspell-0.1.5.7/tests/
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     3710 2022-10-22 18:09:30.000000 hotspell-0.1.5.7/tests/test_heatwaves.py
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2024-05-22 06:21:14.505873 hotspell-0.1.5.8/
+-rw-r--r--   0 ilias     (1000) ilias     (1000)     1557 2021-05-13 12:57:40.000000 hotspell-0.1.5.8/LICENSE
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     2612 2024-05-22 06:21:14.505873 hotspell-0.1.5.8/PKG-INFO
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     2362 2021-09-24 15:19:25.000000 hotspell-0.1.5.8/README.rst
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2024-05-22 06:21:14.501873 hotspell-0.1.5.8/hotspell/
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)       64 2021-08-13 06:22:04.000000 hotspell-0.1.5.8/hotspell/__init__.py
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2024-05-22 06:21:14.505873 hotspell-0.1.5.8/hotspell/datasets/
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)    49328 2022-01-30 14:38:16.000000 hotspell-0.1.5.8/hotspell/datasets/daily_windows_with_length_15.pickle
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)    14192 2022-01-30 14:38:16.000000 hotspell-0.1.5.8/hotspell/datasets/daily_windows_with_length_3.pickle
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)    11730 2024-05-22 06:12:32.000000 hotspell-0.1.5.8/hotspell/heatwaves.py
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     5692 2022-10-22 18:30:31.000000 hotspell-0.1.5.8/hotspell/indices.py
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     3287 2024-05-22 06:15:05.000000 hotspell-0.1.5.8/hotspell/metrics.py
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     2901 2023-11-03 11:17:29.000000 hotspell-0.1.5.8/hotspell/utils.py
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2024-05-22 06:21:14.505873 hotspell-0.1.5.8/hotspell.egg-info/
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     2612 2024-05-22 06:21:14.000000 hotspell-0.1.5.8/hotspell.egg-info/PKG-INFO
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)      418 2024-05-22 06:21:14.000000 hotspell-0.1.5.8/hotspell.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)        1 2024-05-22 06:21:14.000000 hotspell-0.1.5.8/hotspell.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)       13 2024-05-22 06:21:14.000000 hotspell-0.1.5.8/hotspell.egg-info/requires.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)        9 2024-05-22 06:21:14.000000 hotspell-0.1.5.8/hotspell.egg-info/top_level.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)       38 2024-05-22 06:21:14.505873 hotspell-0.1.5.8/setup.cfg
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)      625 2024-05-22 06:19:34.000000 hotspell-0.1.5.8/setup.py
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2024-05-22 06:21:14.505873 hotspell-0.1.5.8/tests/
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     3710 2022-10-22 18:09:30.000000 hotspell-0.1.5.8/tests/test_heatwaves.py
```

### Comparing `hotspell-0.1.5.7/LICENSE` & `hotspell-0.1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.5.7/PKG-INFO` & `hotspell-0.1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotspell
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: Detect heat waves from weather station data
 Home-page: https://github.com/agathangelidis/hotspell
 Author: Ilias Agathangelidis
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 """"""""
```

### Comparing `hotspell-0.1.5.7/README.rst` & `hotspell-0.1.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.5.7/hotspell/datasets/daily_windows_with_length_15.pickle` & `hotspell-0.1.5.8/hotspell/datasets/daily_windows_with_length_15.pickle`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.5.7/hotspell/datasets/daily_windows_with_length_3.pickle` & `hotspell-0.1.5.8/hotspell/datasets/daily_windows_with_length_3.pickle`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.5.7/hotspell/heatwaves.py` & `hotspell-0.1.5.8/hotspell/heatwaves.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     if metrics is True:
         annual_metrics = _get_annual_metrics(
             heatwaves,
             timeseries_ref_period,
             timeseries,
             max_missing_days_pct,
             summer_months,
+            hw_index.var,
         )
     else:
         annual_metrics = None
 
     if export is True:
         _export_heatwaves(heatwaves, filename, hw_index.name)
         if metrics is True:
@@ -164,17 +165,15 @@
         ]
         return df[["window"]]
 
 
 def _import_precomputed_daily_windows(window_length):
     input_file = pkg_resources.resource_filename(
         "hotspell",
-        os.path.join(
-            "datasets", f"daily_windows_with_length_{window_length}.pickle"
-        ),
+        os.path.join("datasets", f"daily_windows_with_length_{window_length}.pickle"),
     )
     df = pd.read_pickle(input_file)
     return df
 
 
 def _add_or_subtract_days(ser, days, op):
     """
@@ -235,17 +234,15 @@
     summer_months : tuple of int
 
     Returns
     -------
     DataFrame
     """
     if summer_months:
-        daily_thresholds = _keep_only_summer(
-            daily_windows.copy(), summer_months
-        )
+        daily_thresholds = _keep_only_summer(daily_windows.copy(), summer_months)
     else:
         daily_thresholds = daily_windows.copy()
 
     if hw_index.pct is not None:
         timeseries_ref_period = timeseries_ref_period.set_index(
             timeseries_ref_period.index.strftime("%m-%d")
         )
@@ -259,34 +256,30 @@
                     hw_index.pct,
                 )
             )
         daily_thresholds["threshold"] = pct_values
     else:
         daily_thresholds["threshold"] = hw_index.fixed_thres
 
-    daily_thresholds = daily_windows.join(
-        daily_thresholds.drop("window", axis=1)
-    )
+    daily_thresholds = daily_windows.join(daily_thresholds.drop("window", axis=1))
     return daily_thresholds
 
 
 def _add_threshold_to_timeseries(timeseries, daily_thresholds):
     """Concatinate the station data and the computed daily thresholds."""
     timeseries = timeseries.asfreq("D")
     df = timeseries.assign(
         date=timeseries.index.strftime("%m-%d"),
         fulldate=timeseries.index.strftime("%Y-%m-%d"),
     ).merge(
         daily_thresholds.assign(
             date=daily_thresholds.index.strftime("%m-%d"), on="date"
         )
     )
-    df = df.sort_values("fulldate").drop(
-        ["date", "fulldate", "window"], axis=1
-    )
+    df = df.sort_values("fulldate").drop(["date", "fulldate", "window"], axis=1)
     df.index = timeseries.index
     return df
 
 
 def _find_heatwaves(timeseries, hw_index, summer_months):
     """
     Find the heat wave dates according to the criteria of a heat wave index.
@@ -323,17 +316,15 @@
     if summer_months:
         heatwaves = _keep_only_summer(heatwaves, summer_months)
 
     return heatwaves
 
 
 def _group_heatwave_days(heatwaves_days):
-    heatwaves_days["group"] = (
-        (heatwaves_days.over.diff(1) != 0).astype("int").cumsum()
-    )
+    heatwaves_days["group"] = (heatwaves_days.over.diff(1) != 0).astype("int").cumsum()
     return heatwaves_days
 
 
 def _compute_heatwave_properties(heatwaves, var, min_duration):
     if min_duration == 1:
         heatwaves = heatwaves[heatwaves["over"].notna()]
     heatwaves["date"] = heatwaves.index
@@ -355,23 +346,19 @@
 
 
 def _filter_with_min_duration(heatwaves, min_duration):
     return heatwaves[heatwaves.duration >= min_duration]
 
 
 def _export_heatwaves(heatwaves, filename, index_name):
-    output_file = (
-        f"{os.path.splitext(filename)[0]}_{index_name}_heatwaves_events.csv"
-    )
+    output_file = f"{os.path.splitext(filename)[0]}_{index_name}_heatwaves_events.csv"
     heatwaves.to_csv(output_file, index=False, date_format="%d/%m/%Y")
 
 
 def _export_annual_metrics(metrics, filename, index_name):
-    output_file = (
-        f"{os.path.splitext(filename)[0]}_{index_name}_heatwaves_metrics.csv"
-    )
+    output_file = f"{os.path.splitext(filename)[0]}_{index_name}_heatwaves_metrics.csv"
     metrics.to_csv(output_file, index=True, date_format="%Y")
 
 
 def _create_output_object(heatwaves, annual_metrics):
     output = HeatWaves(events=heatwaves, metrics=annual_metrics)
     return output
```

### Comparing `hotspell-0.1.5.7/hotspell/indices.py` & `hotspell-0.1.5.8/hotspell/indices.py`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.5.7/hotspell/metrics.py` & `hotspell-0.1.5.8/hotspell/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 def _get_annual_metrics(
     heatwaves,
     timeseries_ref_period,
     timeseries,
     max_missing_days_pct,
     summer_months,
+    var,
 ):
     """
     Calculate the annual heat wave metrics attribute of a HeatWave object.
 
     Parameters
     ----------
     heatwaves : HeatWave object
@@ -27,26 +28,24 @@
     max_missing_days_pct : int
     summer_months : tuple of int
 
     Returns
     -------
     HeatWave object
     """
-    ref_period_mean = _compute_overall_mean(
-        timeseries_ref_period, summer_months
-    )
+    ref_period_mean = _compute_overall_mean(timeseries_ref_period, summer_months)
 
-    annual_metrics = _compute_annual_metrics(heatwaves, ref_period_mean)
+    annual_metrics = _compute_annual_metrics(heatwaves, ref_period_mean, var)
     annual_metrics = _add_valid_years_with_no_heatwaves(
         annual_metrics, timeseries, max_missing_days_pct, summer_months
     )
     return annual_metrics
 
 
-def _compute_annual_metrics(df, ref_period_mean):
+def _compute_annual_metrics(df, ref_period_mean, var):
     hwn = (
         df.groupby([df.index.year], as_index=True)["duration"]
         .count()
         .to_frame(name="hwn")
     )
 
     hwf = (
@@ -65,44 +64,42 @@
         df.groupby([df.index.year], as_index=True)["duration"]
         .mean()
         .to_frame(name="hwdm")
         .round(1)
     )
 
     hwm = (
-        df.groupby([df.index.year], as_index=True)["avg_tmax"]
+        df.groupby([df.index.year], as_index=True)[f"avg_{var}"]
         .mean()
         .to_frame(name="hwm")
         .round(1)
     )
     hwm["hwm"] = np.round(hwm["hwm"] - ref_period_mean, 1)
 
     hwma = (
-        df.groupby([df.index.year], as_index=True)["avg_tmax"]
+        df.groupby([df.index.year], as_index=True)[f"avg_{var}"]
         .mean()
         .to_frame(name="hwma")
         .round(1)
     )
 
     hwa = (
-        df.groupby([df.index.year], as_index=True)["max_tmax"]
+        df.groupby([df.index.year], as_index=True)[f"max_{var}"]
         .max()
         .to_frame(name="hwa")
     )
     hwa["hwa"] = np.round(hwa["hwa"] - ref_period_mean, 1)
 
     hwaa = (
-        df.groupby([df.index.year], as_index=True)["max_tmax"]
+        df.groupby([df.index.year], as_index=True)[f"max_{var}"]
         .max()
         .to_frame(name="hwaa")
     )
 
-    annual_metrics = pd.concat(
-        [hwn, hwf, hwd, hwdm, hwm, hwma, hwa, hwaa], axis=1
-    )
+    annual_metrics = pd.concat([hwn, hwf, hwd, hwdm, hwm, hwma, hwa, hwaa], axis=1)
     annual_metrics.index.rename("year", inplace=True)
 
     return annual_metrics
 
 
 def _add_valid_years_with_no_heatwaves(
     metrics, timeseries, max_missing_days_pct, summer_months
```

### Comparing `hotspell-0.1.5.7/hotspell/utils.py` & `hotspell-0.1.5.8/hotspell/utils.py`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.5.7/hotspell.egg-info/PKG-INFO` & `hotspell-0.1.5.8/hotspell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotspell
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: Detect heat waves from weather station data
 Home-page: https://github.com/agathangelidis/hotspell
 Author: Ilias Agathangelidis
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 """"""""
```

### Comparing `hotspell-0.1.5.7/setup.py` & `hotspell-0.1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="hotspell",
-    version="0.1.5.7",
+    version="0.1.5.8",
     description="Detect heat waves from weather station data",
     author="Ilias Agathangelidis",
     packages=["hotspell"],
     package_data={"hotspell": ["datasets/*.pickle"]},
     install_requires=["numpy", "pandas"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
```

### Comparing `hotspell-0.1.5.7/tests/test_heatwaves.py` & `hotspell-0.1.5.8/tests/test_heatwaves.py`

 * *Files identical despite different names*

