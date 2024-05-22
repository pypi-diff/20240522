# Comparing `tmp/atspm-1.4.0.tar.gz` & `tmp/atspm-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atspm-1.4.0.tar", last modified: Mon May 20 19:54:35 2024, max compression
+gzip compressed data, was "atspm-1.5.0.tar", last modified: Wed May 22 20:04:31 2024, max compression
```

## Comparing `atspm-1.4.0.tar` & `atspm-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.880599 atspm-1.4.0/
--rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.4.0/LICENSE
--rw-rw-rw-   0        0        0       85 2024-04-12 01:08:02.000000 atspm-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3851 2024-05-20 19:54:35.880599 atspm-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3255 2024-05-03 01:09:32.000000 atspm-1.4.0/README.md
--rw-rw-rw-   0        0        0      689 2024-05-20 19:54:26.000000 atspm-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 19:54:35.880599 atspm-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.817701 atspm-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.833329 atspm-1.4.0/src/atspm/
--rw-rw-rw-   0        0        0      117 2024-05-20 19:52:15.000000 atspm-1.4.0/src/atspm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.865095 atspm-1.4.0/src/atspm/data/
--rw-rw-rw-   0        0        0     3321 2024-04-18 18:01:38.000000 atspm-1.4.0/src/atspm/data/sample_config.parquet
--rw-rw-rw-   0        0        0   271222 2024-04-16 00:47:05.000000 atspm-1.4.0/src/atspm/data/sample_raw_data.parquet
--rw-rw-rw-   0        0        0     1938 2024-05-20 19:08:47.000000 atspm-1.4.0/src/atspm/data_aggregator.py
--rw-rw-rw-   0        0        0     2847 2024-05-20 18:20:04.000000 atspm-1.4.0/src/atspm/data_loader.py
--rw-rw-rw-   0        0        0     1326 2024-04-18 17:49:58.000000 atspm-1.4.0/src/atspm/data_saver.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.880599 atspm-1.4.0/src/atspm/queries/
--rw-rw-rw-   0        0        0      348 2024-05-01 17:51:34.000000 atspm-1.4.0/src/atspm/queries/actuations.sql
--rw-rw-rw-   0        0        0     3683 2024-05-01 18:13:20.000000 atspm-1.4.0/src/atspm/queries/arrival_on_green.sql
--rw-rw-rw-   0        0        0      508 2024-05-01 18:16:22.000000 atspm-1.4.0/src/atspm/queries/communications.sql
--rw-rw-rw-   0        0        0      447 2024-05-01 18:22:39.000000 atspm-1.4.0/src/atspm/queries/coordination.sql
--rw-rw-rw-   0        0        0     2537 2024-05-01 22:20:36.000000 atspm-1.4.0/src/atspm/queries/detector_faults.sql
--rw-rw-rw-   0        0        0      907 2024-05-01 16:24:38.000000 atspm-1.4.0/src/atspm/queries/has_data.sql
--rw-rw-rw-   0        0        0      694 2024-05-01 22:26:09.000000 atspm-1.4.0/src/atspm/queries/ped.sql
--rw-rw-rw-   0        0        0    10634 2024-05-02 16:35:05.000000 atspm-1.4.0/src/atspm/queries/split_failures.sql
--rw-rw-rw-   0        0        0      408 2024-05-01 23:51:36.000000 atspm-1.4.0/src/atspm/queries/splits.sql
--rw-rw-rw-   0        0        0      584 2024-05-01 23:54:46.000000 atspm-1.4.0/src/atspm/queries/terminations.sql
--rw-rw-rw-   0        0        0     5613 2024-05-20 16:24:50.000000 atspm-1.4.0/src/atspm/queries/timeline.sql
--rw-rw-rw-   0        0        0     1037 2024-05-01 23:56:18.000000 atspm-1.4.0/src/atspm/queries/unique_ped.sql
--rw-rw-rw-   0        0        0     4724 2024-05-02 00:27:14.000000 atspm-1.4.0/src/atspm/queries/yellow_red.sql
--rw-rw-rw-   0        0        0      493 2024-04-18 18:04:49.000000 atspm-1.4.0/src/atspm/sample_data.py
--rw-rw-rw-   0        0        0     9162 2024-05-20 19:51:05.000000 atspm-1.4.0/src/atspm/signal_data_processor.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.880599 atspm-1.4.0/src/atspm.egg-info/
--rw-rw-rw-   0        0        0     3851 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      881 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 20:04:31.154256 atspm-1.5.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0       85 2024-04-12 01:08:02.000000 atspm-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3874 2024-05-22 20:04:31.151526 atspm-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3255 2024-05-03 01:09:32.000000 atspm-1.5.0/README.md
+-rw-rw-rw-   0        0        0      705 2024-05-22 20:04:00.000000 atspm-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:04:31.154256 atspm-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 20:04:31.024279 atspm-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:04:31.040225 atspm-1.5.0/src/atspm/
+-rw-rw-rw-   0        0        0      117 2024-05-22 16:59:02.000000 atspm-1.5.0/src/atspm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:04:31.072119 atspm-1.5.0/src/atspm/data/
+-rw-rw-rw-   0        0        0     3321 2024-04-18 18:01:38.000000 atspm-1.5.0/src/atspm/data/sample_config.parquet
+-rw-rw-rw-   0        0        0   271222 2024-04-16 00:47:05.000000 atspm-1.5.0/src/atspm/data/sample_raw_data.parquet
+-rw-rw-rw-   0        0        0     2754 2024-05-22 17:22:02.000000 atspm-1.5.0/src/atspm/data_aggregator.py
+-rw-rw-rw-   0        0        0     2898 2024-05-20 23:11:06.000000 atspm-1.5.0/src/atspm/data_loader.py
+-rw-rw-rw-   0        0        0     1326 2024-04-18 17:49:58.000000 atspm-1.5.0/src/atspm/data_saver.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:04:31.149470 atspm-1.5.0/src/atspm/queries/
+-rw-rw-rw-   0        0        0      348 2024-05-01 17:51:34.000000 atspm-1.5.0/src/atspm/queries/actuations.sql
+-rw-rw-rw-   0        0        0     3683 2024-05-01 18:13:20.000000 atspm-1.5.0/src/atspm/queries/arrival_on_green.sql
+-rw-rw-rw-   0        0        0      508 2024-05-01 18:16:22.000000 atspm-1.5.0/src/atspm/queries/communications.sql
+-rw-rw-rw-   0        0        0      447 2024-05-01 18:22:39.000000 atspm-1.5.0/src/atspm/queries/coordination.sql
+-rw-rw-rw-   0        0        0     2537 2024-05-01 22:20:36.000000 atspm-1.5.0/src/atspm/queries/detector_faults.sql
+-rw-rw-rw-   0        0        0     3932 2024-05-22 15:51:16.000000 atspm-1.5.0/src/atspm/queries/full_ped.sql
+-rw-rw-rw-   0        0        0      907 2024-05-01 16:24:38.000000 atspm-1.5.0/src/atspm/queries/has_data.sql
+-rw-rw-rw-   0        0        0      693 2024-05-22 00:16:03.000000 atspm-1.5.0/src/atspm/queries/ped.sql
+-rw-rw-rw-   0        0        0    10634 2024-05-02 16:35:05.000000 atspm-1.5.0/src/atspm/queries/split_failures.sql
+-rw-rw-rw-   0        0        0      408 2024-05-01 23:51:36.000000 atspm-1.5.0/src/atspm/queries/splits.sql
+-rw-rw-rw-   0        0        0      584 2024-05-01 23:54:46.000000 atspm-1.5.0/src/atspm/queries/terminations.sql
+-rw-rw-rw-   0        0        0     5613 2024-05-20 16:24:50.000000 atspm-1.5.0/src/atspm/queries/timeline.sql
+-rw-rw-rw-   0        0        0     1047 2024-05-21 23:53:15.000000 atspm-1.5.0/src/atspm/queries/unique_ped.sql
+-rw-rw-rw-   0        0        0     4724 2024-05-02 00:27:14.000000 atspm-1.5.0/src/atspm/queries/yellow_red.sql
+-rw-rw-rw-   0        0        0      493 2024-04-18 18:04:49.000000 atspm-1.5.0/src/atspm/sample_data.py
+-rw-rw-rw-   0        0        0     8534 2024-05-22 20:01:24.000000 atspm-1.5.0/src/atspm/signal_data_processor.py
+-rw-rw-rw-   0        0        0      650 2024-05-22 17:20:31.000000 atspm-1.5.0/src/atspm/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:04:31.150463 atspm-1.5.0/src/atspm.egg-info/
+-rw-rw-rw-   0        0        0     3874 2024-05-22 20:04:30.000000 atspm-1.5.0/src/atspm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      931 2024-05-22 20:04:31.000000 atspm-1.5.0/src/atspm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:04:30.000000 atspm-1.5.0/src/atspm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-05-22 20:04:30.000000 atspm-1.5.0/src/atspm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-22 20:04:31.000000 atspm-1.5.0/src/atspm.egg-info/top_level.txt
```

### Comparing `atspm-1.4.0/LICENSE` & `atspm-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/PKG-INFO` & `atspm-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: atspm
-Version: 1.4.0
+Version: 1.5.0
 Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb<0.10.2,>=0.9.1
 Requires-Dist: traffic-anomaly>=1.0.0
 Requires-Dist: ibis-framework[duckdb]==9.0.0
+Requires-Dist: jinja2
 
 # ATSPM Aggregation
 
 `atspm` is a Python package to transform hi-res ATC signal controller data into aggregate ATSPMs (Automated Traffic Signal Performance Measures). It works on multiple devices/detectors at once.
 
 ## Installation
```

### Comparing `atspm-1.4.0/README.md` & `atspm-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/pyproject.toml` & `atspm-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atspm"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
   { name="Shawn Strasser", email="shawn.strasser@odot.oregon.gov" },
 ]
 description = "Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -12,15 +12,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "duckdb>=0.9.1,<0.10.2",
     "traffic-anomaly>=1.0.0",
-    "ibis-framework[duckdb]==9.0.0"
+    "ibis-framework[duckdb]==9.0.0",
+    "jinja2",
 ]
 
 [tools.setuptools]
 include_package_data = true
 package_data = {"atspm" = ["queries/*", "data/*"]}
```

### Comparing `atspm-1.4.0/src/atspm/data/sample_config.parquet` & `atspm-1.5.0/src/atspm/data/sample_config.parquet`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/data/sample_raw_data.parquet` & `atspm-1.5.0/src/atspm/data/sample_raw_data.parquet`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/data_aggregator.py` & `atspm-1.5.0/src/atspm/data_aggregator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from jinja2 import Environment, FileSystemLoader
+from .utils import undo_rolling_sum
 
 def render_query(query_name, **kwargs):
     # add from_table = 'raw_data' to the kwargs dictionary
     #kwargs['from_table'] = 'raw_data'
 
     # Get the directory that contains the SQL templates
     template_dir = os.path.join(os.path.dirname(__file__), 'queries')
@@ -32,13 +33,29 @@
         # Drop EventId and Parameter from timeline table
         query += "ALTER TABLE timeline DROP COLUMN EventId; "
         query += "ALTER TABLE timeline DROP COLUMN Parameter; "
         #print(query)
 
 
     try:
+        #print(query)
         conn.execute(query)
+
+        # If agg is full_ped, check if return_volume is True
+        if aggregation_name == 'full_ped':
+            if kwargs['return_volumes']:
+                # Create updated table with the volume data
+                ped_data = conn.sql("SELECT * FROM full_ped").df()
+                ped_data['Estimated_Volumes'] = ped_data.groupby(['DeviceId', 'Phase'])['Estimated_Hourly'].transform(undo_rolling_sum)
+                sql = """
+                    CREATE OR REPLACE TABLE full_ped AS
+                    SELECT * EXCLUDE (Estimated_Hourly)
+                    FROM ped_data
+                    WHERE PedServices >0 OR PedActuation >0 OR Unique_Actuations >0 OR Estimated_Volumes
+                    """
+                conn.sql(sql)
+
     except Exception as e:
         print('Error when executing query for: ', aggregation_name)
         print(e)
         #print('\n\nQuery:\n')
         #print(query)
```

### Comparing `atspm-1.4.0/src/atspm/data_loader.py` & `atspm-1.5.0/src/atspm/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 def load_data(conn,
-              raw_data,
+              raw_data=None,
               detector_config=None,
               unmatched_events=None):
     """
     Loads raw data and detector configuration into DuckDB tables.
 
     This function creates or replaces two tables in the DuckDB database: 'raw_data' and 'detector_config'.
     The data for these tables is loaded from the provided raw_data and detector_config parameters.
@@ -23,18 +23,19 @@
         or a pandas DataFrame containing the unmatched events. If this parameter is None, no unmatched events are loaded.
     """
     # Load Raw Data
     load_sql = """
         CREATE OR REPLACE TABLE raw_data AS
         SELECT TimeStamp, DeviceId, EventId::INT16 as EventId, Parameter::INT16 as Parameter
         """
-    if isinstance(raw_data, str):
-        conn.execute(f"{load_sql} FROM '{raw_data}'")
-    else:
-        conn.execute(f"{load_sql} FROM raw_data")
+    if raw_data is not None:
+        if isinstance(raw_data, str):
+            conn.execute(f"{load_sql} FROM '{raw_data}'")
+        else:
+            conn.execute(f"{load_sql} FROM raw_data")
 
     # Load Configurations (if provided)
     load_sql = """
         CREATE OR REPLACE TABLE detector_config AS
         SELECT DeviceId, Phase::INT16 as Phase, Parameter::INT16 as Parameter, Function::STRING as Function
         """
     if detector_config is not None:
```

### Comparing `atspm-1.4.0/src/atspm/data_saver.py` & `atspm-1.5.0/src/atspm/data_saver.py`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/queries/arrival_on_green.sql` & `atspm-1.5.0/src/atspm/queries/arrival_on_green.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/queries/detector_faults.sql` & `atspm-1.5.0/src/atspm/queries/detector_faults.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/queries/has_data.sql` & `atspm-1.5.0/src/atspm/queries/has_data.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/queries/ped.sql` & `atspm-1.5.0/src/atspm/queries/ped.sql`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 		TimeStamp, 
 		DeviceId, 
 		Parameter::int16 AS Phase, 
 		COALESCE("21", 0)::int16 + COALESCE("67", 0)::int16 AS PedServices, 
 		COALESCE("90", 0)::int16 AS PedActuation
 	FROM (
 		SELECT 
-			TIME_BUCKET(interval '15 minutes', TimeStamp) AS TimeStamp, 
+			TIME_BUCKET(interval '{{bin_size}} minutes', TimeStamp) AS TimeStamp, 
 			DeviceId, 
 			EventId, 
 			Parameter,
 			COUNT(*) AS Total
 		FROM 
 			{{from_table}}
+		WHERE 
+			EventId IN (21, 90, 67)
 		GROUP BY ALL
 	) q
 	PIVOT (
 		SUM(Total) FOR EventID IN (21 AS "21", 90 AS "90", 67 AS "67")
 	)
 ) subquery
-WHERE 
-	PedServices > 0 
-	OR PedActuation > 0
```

### Comparing `atspm-1.4.0/src/atspm/queries/split_failures.sql` & `atspm-1.5.0/src/atspm/queries/split_failures.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/queries/terminations.sql` & `atspm-1.5.0/src/atspm/queries/terminations.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/queries/timeline.sql` & `atspm-1.5.0/src/atspm/queries/timeline.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/queries/unique_ped.sql` & `atspm-1.5.0/src/atspm/queries/unique_ped.sql`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 SELECT
     TimeStamp,
     DeviceId, 
     Phase,
     COUNT(*)::int16 as Unique_Actuations
 FROM
     (SELECT 
-        TIME_BUCKET(interval '15 minutes', TimeStamp) as TimeStamp,
+        TIME_BUCKET(interval '{{bin_size}} minutes', TimeStamp) as TimeStamp,
         DeviceId,
         Parameter::int16 as Phase,
         DATEDIFF('MILLISECOND', LAG(TimeStamp) OVER (PARTITION BY DeviceID, Parameter ORDER BY TimeStamp), TimeStamp)::float as Diff_Milliseconds    
     FROM 
         {{from_table}}
     WHERE
         EventId = 90
```

### Comparing `atspm-1.4.0/src/atspm/queries/yellow_red.sql` & `atspm-1.5.0/src/atspm/queries/yellow_red.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.4.0/src/atspm/signal_data_processor.py` & `atspm-1.5.0/src/atspm/signal_data_processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import duckdb
 import time
-#import importlib
 import traffic_anomaly
-import pandas as pd
 from .data_loader import load_data
 from .data_aggregator import aggregate_data
 from .data_saver import save_data
 
 
 class SignalDataProcessor:
     '''
@@ -32,18 +30,20 @@
     run():
         Loads the data, runs the aggregations, saves the output, and closes the database connection.
     '''
 
     def __init__(self, **kwargs):
         """Initializes the SignalDataProcessor with the provided keyword arguments."""
         # Optional parameters
+        self.raw_data = None
         self.detector_config = None
         self.unmatched_events = None # For timeline aggregation, future use for other aggregations that track phase state (split failure, arrival on green, etc.)
         self.binned_actuations = None # For detector_health aggregation
         self.device_groups = None # For detector_health aggregation if groups are provided
+        self.remove_incomplete = False
         
         # Extract parameters from kwargs
         for key, value in kwargs.items():
             setattr(self, key, value)
 
         # Check for valid bin_size and no_data_min combo
         if self.remove_incomplete:
@@ -52,30 +52,20 @@
             assert self.bin_size % no_data_min == 0, "bin_size / no_data_min must be a whole number"
             # Make sure that has_data is the first aggregation
             idx = [d['name'] for d in self.aggregations].index('has_data')
             self.aggregations.insert(0, self.aggregations.pop(idx))
 
         # Check if detector_health is in aggregations
         if any(d['name'] == 'detector_health' for d in self.aggregations):
-            #print("Detector Health Aggregation Detected.")
-            #try:
-            #    print("Importing traffic-anomaly package...")
-            #    traffic_anomaly = importlib.import_module('traffic_anomaly')
-            #    print(f'traffic-anomaly version: {traffic_anomaly.__version__}')
-            #except ImportError:
-            #    raise ImportError("traffic-anomaly package is required for detector_health aggregation.")
             try:
                 idx = [d['name'] for d in self.aggregations].index('detector_health')
                 self.binned_actuations = self.aggregations[idx]['params']['data']
                 self.device_groups = self.aggregations[idx]['params']['device_groups']
             except KeyError:
-                raise ValueError("detector_health aggregation requires 'data' and 'device_groups' parameters.")
-            # Assert that they are Pandas DataFrames
-            assert isinstance(self.binned_actuations, pd.DataFrame), "binned_actuations must be a Pandas DataFrame"
-            assert isinstance(self.device_groups, pd.DataFrame), "device_groups must be a Pandas DataFrame"
+                raise ValueError("detector_health aggregation requires 'data' and 'device_groups' parameters. 'device_groups' can be set to None.")
      
         # Establish a connection to the database
         self.conn = duckdb.connect()
         # Track whether data has been loaded
         self.data_loaded = False
 
     def load(self):
@@ -93,83 +83,83 @@
         self.data_loaded = True
         self.min_timestamp = self.conn.execute("SELECT MIN(timestamp) FROM raw_data").fetchone()[0]
         self.max_timestamp = self.conn.execute("SELECT MAX(timestamp) FROM raw_data").fetchone()[0]
         print(f'Data loaded from {self.min_timestamp} to {self.max_timestamp}')
         
     def aggregate(self):
         """Runs all aggregations."""
-        if not self.data_loaded:
-            print("Data not loaded! Run the load method first.")
-            return
         # Instantiate a dictionary to store runtimes
         self.runtimes = {}
         for aggregation in self.aggregations:
             start_time = time.time()
-            # Add bin_size and remove_incomplete to params
-            aggregation['params']['bin_size'] = self.bin_size
-            aggregation['params']['remove_incomplete'] = self.remove_incomplete
-            aggregation['params']['from_table'] = 'raw_data'
-
-            ### Detector Faults ###
-            # Add min_timestamp and max_timestamp to params if detector_faults
-            if aggregation['name'] == 'detector_faults':
-                aggregation['params']['min_timestamp'] = self.min_timestamp
-                aggregation['params']['max_timestamp'] = self.max_timestamp
 
+            #######################
             ### Detector Health ###
+            ### Does Not Use aggregate_data function
+            ### Relies on traffic-anomaly package instead
             # Decompose data
             if aggregation['name'] == 'detector_health':
                 decomp = traffic_anomaly.median_decompose(
                     self.binned_actuations,
-                    datetime_column='TimeStamp',
-                    value_column='Total',
-                    entity_grouping_columns=['DeviceId', 'Detector'],
-                    rolling_window_enable=False
+                    **aggregation['params']['decompose_params']
                 )
                 del self.binned_actuations
                 # Join groups to decomp
                 if self.device_groups is not None:
-                    #decomp2 = self.conn.sql("SELECT * FROM decomp NATURAL JOIN self.device_groups").df()
-                    # join with Pandas instead
-                    decomp = decomp.merge(self.device_groups, on=['DeviceId'])
+                    device_groups = self.device_groups # DuckDB needs a direct pointer to see the table
+                    decomp = self.conn.sql("SELECT * FROM decomp NATURAL JOIN device_groups").df()
+                    # Exclude group_grouping_columns in anomaly_params
+                    exclude_col = ', '.join(["'{}'".format(x) for x in aggregation['params']['anomaly_params']['group_grouping_columns']])
+                    exclude_col = f"EXCLUDE ({exclude_col})"
+                    
+                else:
+                    exclude_col = ""
                 # Find Anomalies
                 anomaly = traffic_anomaly.find_anomaly(
                     decomposed_data=decomp,
-                    datetime_column='TimeStamp',
-                    value_column='Total',
-                    entity_grouping_columns=['DeviceId', 'Detector'],
-                    group_grouping_columns=['group'],
-                    entity_threshold=6.0, # using GEH statistic
-                    group_threshold=3.0,
-                    GEH=True,
-                    MAD=False,
-                    log_adjust_negative=True, # exagerate negative values to make them easier to classify as anomalies
+                    **aggregation['params']['anomaly_params']
                 )
                 # Extract max date from anomaly table and subtract return_last_n_days
-                max_date = anomaly['TimeStamp'].max()
-                max_date = max_date - pd.Timedelta(days=aggregation['params']['return_last_n_days'])
-                # convert to date string
-                max_date = max_date.strftime('%Y-%m-%d')
-                
+                sql = f"""
+                    SELECT CAST(MAX(TimeStamp)::DATE - INTERVAL '{aggregation['params']['return_last_n_days']-1}' DAY AS VARCHAR) AS max_date_minus_one
+                    FROM anomaly
+                    """
+                max_date = self.conn.query(sql).fetchone()[0]
+
                 # Save anomaly table to DuckDB
                 query = f"""CREATE OR REPLACE TABLE detector_health AS
-                        SELECT * FROM anomaly
+                        SELECT * {exclude_col}
+                        FROM anomaly
                         WHERE TimeStamp >= '{max_date}'
                         """
                 self.conn.execute(query)
-                # no external sql file for detector_health
+                # no external sql file like other aggregations, so just continue
                 end_time = time.time()
                 self.runtimes[aggregation['name']] = end_time - start_time
                 continue
 
+            # Add bin_size and remove_incomplete to params
+            aggregation['params']['bin_size'] = self.bin_size
+            aggregation['params']['remove_incomplete'] = self.remove_incomplete
+            aggregation['params']['from_table'] = 'raw_data'
+
+            #######################
+            ### Detector Faults / Full Pedestrian ###
+            # Add min_timestamp and max_timestamp to params if detector_faults or full_ped
+            if aggregation['name'] == 'detector_faults' or aggregation['name'] == 'full_ped':
+                aggregation['params']['min_timestamp'] = self.min_timestamp
+                aggregation['params']['max_timestamp'] = self.max_timestamp
+
+            #######################
             ### Timeline ##########
             # If timeline and self.unmatched_events is not None, update from_table to 'all_events' view
             if aggregation['name'] == 'timeline' and self.unmatched_events is not None:
                 aggregation['params']['from_table'] = 'all_events'
 
+            #######################
             ### Run Aggregation ###
             aggregate_data(self.conn,
                     aggregation['name'],
                     **aggregation['params'])
             end_time = time.time()
             self.runtimes[aggregation['name']] = end_time - start_time
```

### Comparing `atspm-1.4.0/src/atspm.egg-info/PKG-INFO` & `atspm-1.5.0/src/atspm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: atspm
-Version: 1.4.0
+Version: 1.5.0
 Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb<0.10.2,>=0.9.1
 Requires-Dist: traffic-anomaly>=1.0.0
 Requires-Dist: ibis-framework[duckdb]==9.0.0
+Requires-Dist: jinja2
 
 # ATSPM Aggregation
 
 `atspm` is a Python package to transform hi-res ATC signal controller data into aggregate ATSPMs (Automated Traffic Signal Performance Measures). It works on multiple devices/detectors at once.
 
 ## Installation
```

### Comparing `atspm-1.4.0/src/atspm.egg-info/SOURCES.txt` & `atspm-1.5.0/src/atspm.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 pyproject.toml
 src/atspm/__init__.py
 src/atspm/data_aggregator.py
 src/atspm/data_loader.py
 src/atspm/data_saver.py
 src/atspm/sample_data.py
 src/atspm/signal_data_processor.py
+src/atspm/utils.py
 src/atspm.egg-info/PKG-INFO
 src/atspm.egg-info/SOURCES.txt
 src/atspm.egg-info/dependency_links.txt
 src/atspm.egg-info/requires.txt
 src/atspm.egg-info/top_level.txt
 src/atspm/data/sample_config.parquet
 src/atspm/data/sample_raw_data.parquet
 src/atspm/queries/actuations.sql
 src/atspm/queries/arrival_on_green.sql
 src/atspm/queries/communications.sql
 src/atspm/queries/coordination.sql
 src/atspm/queries/detector_faults.sql
+src/atspm/queries/full_ped.sql
 src/atspm/queries/has_data.sql
 src/atspm/queries/ped.sql
 src/atspm/queries/split_failures.sql
 src/atspm/queries/splits.sql
 src/atspm/queries/terminations.sql
 src/atspm/queries/timeline.sql
 src/atspm/queries/unique_ped.sql
```

