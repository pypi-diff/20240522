# Comparing `tmp/onetick_latency-0.1.2.tar.gz` & `tmp/onetick_latency-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetick_latency-0.1.2.tar", last modified: Tue May 21 20:44:45 2024, max compression
+gzip compressed data, was "onetick_latency-0.1.3.tar", last modified: Wed May 22 13:20:00 2024, max compression
```

## Comparing `onetick_latency-0.1.2.tar` & `onetick_latency-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.562859 onetick_latency-0.1.2/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.2/modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.2/modules/cross_over_controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8128 2024-05-17 14:52:06.000000 onetick_latency-0.1.2/modules/latency_module.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.2/modules/volume_analyser.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/onetick_latency.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-21 20:44:45.000000 onetick_latency-0.1.2/onetick_latency.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/pythonAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.2/pythonAPI/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-21 20:30:57.000000 onetick_latency-0.1.2/pythonAPI/auth.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3133 2024-05-21 20:44:01.000000 onetick_latency-0.1.2/pythonAPI/runnbboquote.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-05-21 20:16:37.000000 onetick_latency-0.1.2/pythonAPI/security_credentials.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-21 20:44:45.566859 onetick_latency-0.1.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-21 20:44:43.000000 onetick_latency-0.1.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2024-05-17 15:17:01.000000 onetick_latency-0.1.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.577139 onetick_latency-0.1.3/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.3/modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2474 2024-05-17 14:52:06.000000 onetick_latency-0.1.3/modules/cross_over_controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8130 2024-05-22 12:58:34.000000 onetick_latency-0.1.3/modules/latency_module.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5571 2024-05-17 14:52:06.000000 onetick_latency-0.1.3/modules/volume_analyser.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.577139 onetick_latency-0.1.3/onetick_latency.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2932 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-22 13:20:00.000000 onetick_latency-0.1.3/onetick_latency.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/pythonAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 17:42:00.000000 onetick_latency-0.1.3/pythonAPI/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-21 20:30:57.000000 onetick_latency-0.1.3/pythonAPI/auth.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3031 2024-05-22 13:17:53.000000 onetick_latency-0.1.3/pythonAPI/runnbboquote.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-05-21 20:16:37.000000 onetick_latency-0.1.3/pythonAPI/security_credentials.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 13:20:00.581139 onetick_latency-0.1.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2024-05-22 13:18:48.000000 onetick_latency-0.1.3/setup.py
```

### Comparing `onetick_latency-0.1.2/PKG-INFO` & `onetick_latency-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick_latency
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.2/README.md` & `onetick_latency-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.2/modules/cross_over_controller.py` & `onetick_latency-0.1.3/modules/cross_over_controller.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.2/modules/latency_module.py` & `onetick_latency-0.1.3/modules/latency_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         }
 
         print("\n--------------------LATENCY PARAMETERS------------------------------")
         print("Initial Latency Parameters Set:")
         for key, value in self.latency_params.items():
             print(f"  {key}: {value}\n")
 
-
         self.cross_control = CrossOverController(self.df)
 
 
     def get_high_latency_periods(self):
         """
         Retrieve high latency periods from the volume analyzer and format them for latency simulation.
 
@@ -90,36 +89,39 @@
             end_hour = pd.to_datetime(period['End']).hour + pd.to_datetime(period['End']).minute / MINUTES_IN_HOUR
             latency_periods.append((start_hour, end_hour, period['Delta from Mean (%)']))
 
             print(f"\nFrom {period['Start']} to {period['End']} with {period['quote Count']} quotes, Average Delta: {period['Delta from Mean (%)']:.2f}%")
 
         return latency_periods
 
+
     def generate_latency_factors(self):
         """
         Precompute latency factors for each timestamp in the DataFrame based on high latency periods.
         """
         if self.df.empty or 'Time' not in self.df.columns:
             raise ValueError("DataFrame is empty or missing required 'Time' column.")
 
         self.df['hour_of_day'] = self.df['Time'].dt.hour + self.df['Time'].dt.minute / MINUTES_IN_HOUR
         self.df['latency_factor'] = LATENCY_FACTOR
         for start, end, increase in self.latency_params['high_latency_periods']:
             self.df.loc[(self.df['hour_of_day'] >= start) & (self.df['hour_of_day'] < end), 'latency_factor'] += increase / PERCENTAGE
 
+
     def report_simulation_metrics(self):
         """
         Report metrics such as mean and standard deviation of the simulated latencies.
         """
         simulated_mean = np.mean(self.df['latency_ns'])
         simulated_std = np.std(self.df['latency_ns'])
         print("\n----------------------SIMULATION METRICS---------------------------------\n")
         print(f"Simulated Mean Latency: {simulated_mean} ns")
         print(f"Simulated Standard Deviation: {simulated_std} ns")
 
+
     def adjust_timestamps(self):
         """
         Adjust the timestamps in the DataFrame by applying the generated latency values,
         ensuring each timestamp reflects realistic network delays while maintaining specified statistical properties.
         """
         self.generate_latency_factors()
 
@@ -165,15 +167,14 @@
         plt.hist(self.df['latency_ns'], bins=BIN_FOR_PLOT, color='blue', alpha=ALPHA_FOR_PLOT)
         plt.title('Latency Distribution')
         plt.xlabel('Latency (ns)')
         plt.ylabel('Frequency')
         plt.show()
 
 
-
 if __name__ == '__main__':
     simulator = NetworkSimulator(
         from_date='2024-05-08',
         to_date='2024-05-11',
         symbol='QQQT',
         batch_size=20,
         timezone='America/New_York',
```

### Comparing `onetick_latency-0.1.2/modules/volume_analyser.py` & `onetick_latency-0.1.3/modules/volume_analyser.py`

 * *Files identical despite different names*

### Comparing `onetick_latency-0.1.2/onetick_latency.egg-info/PKG-INFO` & `onetick_latency-0.1.3/onetick_latency.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetick-latency
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library for latency simulation and query for Onetick
 Home-page: https://gitlab.awsged.com/bigdata/onetick_latency.git
 Author: Alexandre Levert
 Author-email: alexandre.levert.1@bnc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `onetick_latency-0.1.2/pythonAPI/runnbboquote.py` & `onetick_latency-0.1.3/pythonAPI/runnbboquote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-import sys
-import os
-
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 import onetick.query as otq
 from onetick_latency.creds import dir_home, current_dir, username_authentication, password_authentication
 import pandas as pd
 import time
 import datetime as dt
 import pytz
```

### Comparing `onetick_latency-0.1.2/setup.py` & `onetick_latency-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Safely read the long description from 'README.md'
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='onetick_latency',
-    version='0.1.2',
+    version='0.1.3',
     description='Library for latency simulation and query for Onetick',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alexandre Levert',
     author_email='alexandre.levert.1@bnc.ca',
     url='https://gitlab.awsged.com/bigdata/onetick_latency.git',
     packages=find_packages(include=['onetick_latency*', 'modules*', 'pythonAPI*']),
```

