# Comparing `tmp/onetick_latency-0.1.6.tar.gz` & `tmp/onetick_latency-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetick_latency-0.1.6.tar", last modified: Wed May 22 15:13:15 2024, max compression
+gzip compressed data, was "onetick_latency-0.1.7.tar", last modified: Wed May 22 17:30:22 2024, max compression
```

## Comparing `onetick_latency-0.1.6.tar` & `onetick_latency-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:13:15.520500 onetick_latency-0.1.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 15:13:15.520500 onetick_latency-0.1.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:13:15.520500 onetick_latency-0.1.6/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.6/modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.6/modules/cross_over_controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8098 2024-05-22 15:12:17.000000 onetick_latency-0.1.6/modules/latency_module.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.6/modules/volume_analyser.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:13:15.520500 onetick_latency-0.1.6/onetick_latency.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 15:13:15.000000 onetick_latency-0.1.6/onetick_latency.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2024-05-22 15:13:15.000000 onetick_latency-0.1.6/onetick_latency.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 15:13:15.000000 onetick_latency-0.1.6/onetick_latency.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 15:13:15.000000 onetick_latency-0.1.6/onetick_latency.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 15:13:15.000000 onetick_latency-0.1.6/onetick_latency.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 15:13:15.520500 onetick_latency-0.1.6/pythonAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.6/pythonAPI/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-22 13:17:27.000000 onetick_latency-0.1.6/pythonAPI/auth.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2024-05-22 15:07:25.000000 onetick_latency-0.1.6/pythonAPI/creds.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3000 2024-05-22 13:47:36.000000 onetick_latency-0.1.6/pythonAPI/runnbboquote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 15:13:15.520500 onetick_latency-0.1.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 15:13:12.000000 onetick_latency-0.1.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2618 2024-05-22 17:28:52.000000 onetick_latency-0.1.7/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.7/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.7/modules/cross_over_controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8197 2024-05-22 17:28:52.000000 onetick_latency-0.1.7/modules/latency_module.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.7/modules/volume_analyser.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/onetick_latency.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      366 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 17:30:22.000000 onetick_latency-0.1.7/onetick_latency.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/pythonAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.7/pythonAPI/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2024-05-22 15:56:30.000000 onetick_latency-0.1.7/pythonAPI/runnbboquote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 17:30:22.984658 onetick_latency-0.1.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 17:29:23.000000 onetick_latency-0.1.7/setup.py
```

### Comparing `onetick_latency-0.1.6/PKG-INFO` & `onetick_latency-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick_latency
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -21,29 +21,31 @@
 This library has various fonctionnality such a latency simulator as well as a query script for querying nbbo data from 
 OneTick software. 
 
 ## Installation and requirements
 
 This library requires OneTick software installed.
 
-- [ ] pip install the wheel for this package
-- [ ] pip install the requirements for this package
+- [ ] pip install onetick-latency module
+- [ ] pip install the requirements.txt for this package
 
 
 ## Latency Module
 The Latency module is designed to simulate network latency based on trading volumes and activity. It adjusts DataFrame timestamps to mimic realistic network delays by applying generated latency values drawn from a Gaussian normal distribution.
 
 ### Key Features:
 
 - Flexible parameter inputs including date range (format: "yyyy-mm-dd") , symbol, batch size, and timezone.
 - Configurable min/max latency values to reflect observed extremes.
 - Mean and standard deviation settings for latency mirroring observed data characteristics.
 - Jitter factor to simulate real-life network behavior.
 - Options to plot latency distributions and trading volume over time.
 - Metrics display for simulation analysis.
+- Specify onetick_directory path and working_directory for otq file and saving to pickle the query
+- Specify onetick credentials as parameters of the class (strongly suggest to do a file and import the user and password)
 
 ## Timestamp Crossover Module
 This module detects timestamp anomalies where entries are out of chronological order—a common issue in high-frequency trading data that can lead to significant analytical errors.
 
 ### Functionality:
 
 - Identifies and reports rows where timestamps are not sequential.
```

### Comparing `onetick_latency-0.1.6/README.md` & `onetick_latency-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 This library has various fonctionnality such a latency simulator as well as a query script for querying nbbo data from 
 OneTick software. 
 
 ## Installation and requirements
 
 This library requires OneTick software installed.
 
-- [ ] pip install the wheel for this package
-- [ ] pip install the requirements for this package
+- [ ] pip install onetick-latency module
+- [ ] pip install the requirements.txt for this package
 
 
 ## Latency Module
 The Latency module is designed to simulate network latency based on trading volumes and activity. It adjusts DataFrame timestamps to mimic realistic network delays by applying generated latency values drawn from a Gaussian normal distribution.
 
 ### Key Features:
 
 - Flexible parameter inputs including date range (format: "yyyy-mm-dd") , symbol, batch size, and timezone.
 - Configurable min/max latency values to reflect observed extremes.
 - Mean and standard deviation settings for latency mirroring observed data characteristics.
 - Jitter factor to simulate real-life network behavior.
 - Options to plot latency distributions and trading volume over time.
 - Metrics display for simulation analysis.
+- Specify onetick_directory path and working_directory for otq file and saving to pickle the query
+- Specify onetick credentials as parameters of the class (strongly suggest to do a file and import the user and password)
 
 ## Timestamp Crossover Module
 This module detects timestamp anomalies where entries are out of chronological order—a common issue in high-frequency trading data that can lead to significant analytical errors.
 
 ### Functionality:
 
 - Identifies and reports rows where timestamps are not sequential.
```

### Comparing `onetick_latency-0.1.6/modules/cross_over_controller.py` & `onetick_latency-0.1.7/modules/cross_over_controller.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.6/modules/latency_module.py` & `onetick_latency-0.1.7/modules/latency_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,48 +2,44 @@
 Network Simulation Module
 Developed by Alexandre Levert, NBC (National Bank du Canada)
 May 2024
 
 This module simulates network latency based on trading activity and high-activity periods identified
 by the VolumeAnalyser. It uses the DataFrame of trading data to adjust timestamps based on calculated latencies.
 """
-import sys
-import os
 
-# Append the parent directory to sys.path
-parent_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
-sys.path.append(parent_dir)
-
-from pythonAPI.runnbboquote import OneTickQueryRunner
+from onetick_latency.pythonAPI.runnbboquote import OneTickQueryRunner
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from modules.volume_analyser import VolumeAnalyser
 from modules.cross_over_controller import CrossOverController
 
 MINUTES_IN_HOUR = 60
 PERCENTAGE = 100
 LATENCY_FACTOR = 1.0
 BIN_FOR_PLOT = 50
 ALPHA_FOR_PLOT = 0.7
 
 class NetworkSimulator:
     def __init__(self, from_date, to_date, symbol, batch_size, timezone, volume_analyser_min, volume_analyser_percentile,
-                 min_latency_ns, max_latency_ns, mean_latency_ns, std_dev_ns, jitter_factor, plot_latency=False,
-                 plot_quotes=False, show_metrics=True, otq_file_path=None, save_to_pickle=False, pickle_path=None):
+                 min_latency_ns, max_latency_ns, mean_latency_ns, std_dev_ns, jitter_factor,username, password,
+                 onetick_dir="/home/ubuntu/onetick-onboarding/onetick",working_dir="/home/ubuntu/projects/onetick_latency",
+                 plot_latency=False,plot_quotes=False, show_metrics=True, otq_file_path=None,
+                 save_to_pickle=False, pickle_path=None):
         """
         Initialize the Network Simulator with all parameters needed for simulation.
 
         Parameters:
         - All necessary parameters for setting up and running the latency simulation.
         """
         self.plot_latency = plot_latency
         self.plot_quotes = plot_quotes
         self.show_metrics = show_metrics
-        self.query_runner = OneTickQueryRunner()
+        self.query_runner = OneTickQueryRunner(username, password, onetick_dir, working_dir)
         self.df = self.query_runner.run_market(
             from_date=from_date,
             to_date=to_date,
             symbol=symbol,
             batch_size=batch_size,
             timezone=timezone,
             otq_file_path=otq_file_path,
@@ -181,14 +177,16 @@
         volume_analyser_min=5,
         volume_analyser_percentile=80,
         min_latency_ns=40,
         max_latency_ns=1200,
         mean_latency_ns=150,
         std_dev_ns=20,
         jitter_factor=0.15,
+        username='user',
+        password='pass',
         plot_latency=True,
         plot_quotes=True,
         show_metrics=True
     )
     simulator.adjust_timestamps()
     print(simulator.df.tail(20))
```

### Comparing `onetick_latency-0.1.6/modules/volume_analyser.py` & `onetick_latency-0.1.7/modules/volume_analyser.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.6/onetick_latency.egg-info/PKG-INFO` & `onetick_latency-0.1.7/onetick_latency.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick-latency
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -21,29 +21,31 @@
 This library has various fonctionnality such a latency simulator as well as a query script for querying nbbo data from 
 OneTick software. 
 
 ## Installation and requirements
 
 This library requires OneTick software installed.
 
-- [ ] pip install the wheel for this package
-- [ ] pip install the requirements for this package
+- [ ] pip install onetick-latency module
+- [ ] pip install the requirements.txt for this package
 
 
 ## Latency Module
 The Latency module is designed to simulate network latency based on trading volumes and activity. It adjusts DataFrame timestamps to mimic realistic network delays by applying generated latency values drawn from a Gaussian normal distribution.
 
 ### Key Features:
 
 - Flexible parameter inputs including date range (format: "yyyy-mm-dd") , symbol, batch size, and timezone.
 - Configurable min/max latency values to reflect observed extremes.
 - Mean and standard deviation settings for latency mirroring observed data characteristics.
 - Jitter factor to simulate real-life network behavior.
 - Options to plot latency distributions and trading volume over time.
 - Metrics display for simulation analysis.
+- Specify onetick_directory path and working_directory for otq file and saving to pickle the query
+- Specify onetick credentials as parameters of the class (strongly suggest to do a file and import the user and password)
 
 ## Timestamp Crossover Module
 This module detects timestamp anomalies where entries are out of chronological order—a common issue in high-frequency trading data that can lead to significant analytical errors.
 
 ### Functionality:
 
 - Identifies and reports rows where timestamps are not sequential.
```

### Comparing `onetick_latency-0.1.6/pythonAPI/runnbboquote.py` & `onetick_latency-0.1.7/pythonAPI/runnbboquote.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import onetick.query as otq
-from pythonAPI.creds import dir_home, current_dir, username_authentication
+import os
 import pandas as pd
 import time
 import datetime as dt
 import pytz
 
 class OneTickQueryRunner:
 
-    def __init__(self, context="DEFAULT"):
+    def __init__(self, username_authentication, password_authentication,onetick_dir, working_dir, context="DEFAULT"):
         self.context = context
+        self.onetick_dir = onetick_dir
+        self.working_dir = working_dir
+        self.onetick_lib = otq.OneTickLib(None)
+        self.username_authentication = self.onetick_lib.set_username_for_authentication(username_authentication)
+        self.password = self.onetick_lib.set_password(password_authentication)
+        self.env = os.environ["ONE_TICK_CONFIG"] = f"{self.onetick_dir}/client_data/config/one_tick_config.txt"  # point to OneTick main config file on your local machine
+
 
     def run_query(self, query, query_timezone, params, save_to_pickle, pickle_path):
         current_time = dt.datetime.now(pytz.timezone(query_timezone))
         print(f"{current_time}: run_query: context: {self.context}: starting")
 
         tic = time.time()
         query_result = otq.run(
             query,
-            username=username_authentication,
+            username=self.username_authentication,
             context=self.context,
             query_params=params,
             timezone=query_timezone,
             time_as_nsec=True
         )
         toc = time.time()
         df = self.print_query_result(query_result, save_to_pickle, pickle_path)
@@ -45,36 +52,23 @@
         return df
 
     def extract_symbol(self, name):
         return name.split("::")[-1] if "::" in name else name
 
     def run_market(self, from_date, to_date, symbol, batch_size, timezone, otq_file_path=None, save_to_pickle=True, pickle_path=None):
         if otq_file_path is None:
-            otq_file_path = f"{dir_home}/client_data/otqs/NBBO.otq::soni"  # default OTQ file path
+            otq_file_path = f"{self.onetick_dir}/client_data/otqs/NBBO.otq::soni"  # default OTQ file path
         if pickle_path is None:
-            pickle_path = f"{current_dir}/modules"  # default pickle save path
+            pickle_path = f"{self.working_dir}/modules"  # default pickle save path
 
         params = {
             "START_TIME": from_date.replace('-', '') + "000000",
             "END_TIME": to_date.replace('-', '') + "235959",
             "SYMBOL_PATTERN": symbol,
             "BATCH_SIZE": str(batch_size),
             "time_zone": timezone
         }
         df = self.run_query(query=otq_file_path, params=params, query_timezone=timezone, save_to_pickle=save_to_pickle, pickle_path=pickle_path)
         print("Success for HITS JOB\n")
 
 
-        return df
-
-if __name__ == '__main__':
-    query_runner = OneTickQueryRunner()
-    query_runner.run_market(
-        from_date='2024-05-10',
-        to_date='2024-05-12',
-        symbol='XIU',
-        batch_size=20,
-        timezone='America/New_York',
-        otq_file_path=None,  # default will be used
-        save_to_pickle=True,
-        pickle_path=None  # default will be used
-    )
+        return df
```

### Comparing `onetick_latency-0.1.6/setup.py` & `onetick_latency-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Safely read the long description from 'README.md'
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='onetick_latency',
-    version='0.1.6',
+    version='0.1.7',
     description='Library for latency simulation and query for Onetick',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alexandre Levert',
     author_email='alexandre.levert.1@bnc.ca',
     url='https://gitlab.awsged.com/bigdata/onetick_latency.git',
     packages=find_packages(include=['onetick_latency*', 'modules*', 'pythonAPI*']),
```

