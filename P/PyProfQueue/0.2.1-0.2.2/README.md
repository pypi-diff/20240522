# Comparing `tmp/PyProfQueue-0.2.1.tar.gz` & `tmp/PyProfQueue-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.2.1.tar", last modified: Wed May 22 12:13:03 2024, max compression
+gzip compressed data, was "PyProfQueue-0.2.2.tar", last modified: Wed May 22 12:40:28 2024, max compression
```

## Comparing `PyProfQueue-0.2.1.tar` & `PyProfQueue-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.658128 PyProfQueue-0.2.1/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23306 2024-05-22 12:13:03.658128 PyProfQueue-0.2.1/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      404 2024-05-22 12:10:27.000000 PyProfQueue-0.2.1/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue/profilers/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/__init__.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2377 2024-05-14 16:15:39.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/_template_profiler.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue/profilers/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/_template_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1711 2024-05-22 12:01:34.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1643 2024-05-22 12:01:34.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     8023 2024-05-22 11:58:30.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/likwid.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14926 2024-05-22 11:20:22.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    39177 2024-05-22 11:10:00.000000 PyProfQueue-0.2.1/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.1/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23306 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      619 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.1/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-22 12:13:03.658128 PyProfQueue-0.2.1/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1506 2024-05-22 12:10:27.000000 PyProfQueue-0.2.1/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:40:28.322998 PyProfQueue-0.2.2/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23306 2024-05-22 12:40:28.322998 PyProfQueue-0.2.2/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:40:28.322998 PyProfQueue-0.2.2/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      404 2024-05-22 12:40:19.000000 PyProfQueue-0.2.2/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:40:28.322998 PyProfQueue-0.2.2/PyProfQueue/profilers/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/__init__.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2377 2024-05-14 16:15:39.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/_template_profiler.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:40:28.322998 PyProfQueue-0.2.2/PyProfQueue/profilers/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/data/_template_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1709 2024-05-22 12:36:52.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1247 2024-05-22 12:38:47.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     8023 2024-05-22 11:58:30.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/likwid.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14893 2024-05-22 12:39:54.000000 PyProfQueue-0.2.2/PyProfQueue/profilers/prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    40332 2024-05-22 12:38:46.000000 PyProfQueue-0.2.2/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.2/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:40:28.322998 PyProfQueue-0.2.2/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23306 2024-05-22 12:40:28.000000 PyProfQueue-0.2.2/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      619 2024-05-22 12:40:28.000000 PyProfQueue-0.2.2/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-22 12:40:28.000000 PyProfQueue-0.2.2/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-22 12:40:28.000000 PyProfQueue-0.2.2/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-22 12:40:28.000000 PyProfQueue-0.2.2/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.2/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-22 12:40:28.322998 PyProfQueue-0.2.2/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1506 2024-05-22 12:40:19.000000 PyProfQueue-0.2.2/setup.py
```

### Comparing `PyProfQueue-0.2.1/PKG-INFO` & `PyProfQueue-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.1/PyProfQueue/profilers/_template_profiler.py` & `PyProfQueue-0.2.2/PyProfQueue/profilers/_template_profiler.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.1/PyProfQueue/profilers/data/likwid_commands.txt` & `PyProfQueue-0.2.2/PyProfQueue/profilers/data/likwid_commands.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 echo 'Scalar MFlops/s' > ${LIK_OUTPUT}
 likwid-bench -t peakflops -W N:${STREAM_SIZE}:${THREAD_COUNT} | grep 'MFlops/s:' >> ${LIK_OUTPUT}
 echo 'SSE MFlops/s' >> ${LIK_OUTPUT}
 likwid-bench -t peakflops_sse -W N:${STREAM_SIZE}:${THREAD_COUNT} | grep 'MFlops/s:' >> ${LIK_OUTPUT}
 echo 'AVX MFlops/s' >> ${LIK_OUTPUT}
 likwid-bench -t peakflops_avx -W N:${STREAM_SIZE}:${THREAD_COUNT} | grep 'MFlops/s:' >> ${LIK_OUTPUT}
 echo 'Scalar MByte/s' >> ${LIK_OUTPUT}
-export BEST_PERF=grep -oP 'MFlops/s:\s*\K\d+' ${LIK_OUTPUT} | sort -n | tail -n 1
+export BEST_PERF=$(grep -oP 'MFlops/s:\s*\K\d+' ${LIK_OUTPUT} | sort -n | tail -n 1)
 
 likwid-bench -t load -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 echo 'SSE MByte/s' >> ${LIK_OUTPUT}
 likwid-bench -t load_sse -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 echo 'AVX MByte/s' >> ${LIK_OUTPUT}
 likwid-bench -t load_avx -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
-export BEST_BAND=grep -oP 'MByte/s:\s*\K\d+' ${LIK_OUTPUT} | sort -n | tail -n 1
-
+export BEST_BAND=$(grep -oP 'MByte/s:\s*\K\d+' ${LIK_OUTPUT} | sort -n | tail -n 1)
 # *=*
 sleep 1
 echo 'Program Performance' >> ${LIK_OUTPUT}
 grep -e 'MFLOP/s STAT' -e 'Operational intensity STAT' ${WORKING_DIR}/job_output_setup.txt >> ${LIK_OUTPUT}
 
 # Check if cwl file exists to call the script with that file
-export
 ${PYTHON_INSTANCE} -c "import PyProfQueue.profilers.likwid as lik;"\
 "lik.plot_roof_timeseries(likwid_file='${LIKWID_RUNNING_DIR}/likwid_output.txt', "\
 "name_prefix='${WORKING_DIR}/Likwid', maxperf=${BEST_PERF}, maxband=${BEST_BAND})"
```

### Comparing `PyProfQueue-0.2.1/PyProfQueue/profilers/data/prometheus_commands.txt` & `PyProfQueue-0.2.2/PyProfQueue/profilers/data/prometheus_commands.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 mkdir ${PROMETHEUS_RUNNING_DIR}
 # *=*
 ${PROMETHEUS_SOFTWARE}/prometheus/prometheus --config.file=${PROMETHEUS_SOFTWARE}/prometheus/prometheus.yml --storage.tsdb.path=${PROMETHEUS_RUNNING_DIR}/data > /dev/null 2>&1 &
 export PROMETHEUS_PID=$!
 ${PROMETHEUS_SOFTWARE}/node_exporter/node_exporter > /dev/null 2>&1 &
 export NODE_PID=$!
 # *=*
-export START_TIME=$(date +%s)
-sleep 10
-# *=*
-sleep 10
-export END_TIME=$(date +%s)
-export DURATION=$((${END_TIME} - ${START_TIME}))
-export START=$(date -d @${START_TIME} +"%Y-%m-%d %H:%M:%S")
-export END=$(date -d @${END_TIME} +"%Y-%m-%d %H:%M:%S")
 ${PYTHON_INSTANCE} ${PROFILE_SCRAPE}/read_prometheus.py -o "${PROMETHEUS_RUNNING_DIR}" -s "${START}" -e "${END}" -i "${PROMETHEUS_IP}"
 # *=*
 sleep 1
 kill -TERM ${NODE_PID}
 kill -TERM ${PROMETHEUS_PID}
 # *=*
-echo 'Run time: '$((${DURATION}/60/60))':'$((${DURATION}/60%60 ))':'$((${DURATION}%60))
 echo 'Plotting Prometheus metrics to ${PROMETHEUS_RUNNING_DIR}'
-
-# Check if cwl file exists to call the script with that file
 if [ -f ${WORKING_DIR}/job_output_setup.txt ]; then
     ${PYTHON_INSTANCE} -c "import PyProfQueue.profilers.prometheus as prom;"\
     "df, time_series = prom.load_df('${WORKING_DIR}/Prometheus/prometheus_data');"\
     "prom.plot_prom_profiling(df=df, time_series=time_series, name_prefix='${WORKING_DIR}/Prometheus', cwl_file='${WORKING_DIR}/job_output_setup.txt')"
 else
     ${PYTHON_INSTANCE} -c "import PyProfQueue.profilers.prometheus as prom;"\
     "df, time_series = prom.load_df('${WORKING_DIR}/Prometheus/prometheus_data');"\
     "prom.plot_prom_profiling(df=df, time_series=time_series, name_prefix='${WORKING_DIR}/Prometheus')"
-fi
+fi
```

### Comparing `PyProfQueue-0.2.1/PyProfQueue/profilers/data/read_prometheus.py` & `PyProfQueue-0.2.2/PyProfQueue/profilers/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.1/PyProfQueue/profilers/likwid.py` & `PyProfQueue-0.2.2/PyProfQueue/profilers/likwid.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.1/PyProfQueue/profilers/prometheus.py` & `PyProfQueue-0.2.2/PyProfQueue/profilers/prometheus.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,28 +54,29 @@
     else:
         IP_address = profilerdict['ip_address']
         profilefile.write(f"export PROMETHEUS_IP={IP_address}\n")
     profilefile.write('export PROMETHEUS_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
     scrape_path = str(impresources.path(data, 'read_prometheus.py'))[:-19]
     profilefile.write('export PROFILE_SCRAPE={}\n'.format(scrape_path))
     profilefile.write('\n')
-    final_init_indicator = 2
+    final_init_indicator = 1
     if IP_address is None:
-        read_indicators = [0, 1, 2]
+        read_indicators = [0, 1]
     else:
-        read_indicators = [0, 2]
+        read_indicators = [0]
     indicator = 0
     with open(prometheus_file_path, 'r') as read_file:
         for number, line in enumerate(read_file):
             if line == '# *=*\n' and indicator >= final_init_indicator:
                 prometheus_initEndSplit = number + 1
                 break
             elif line == '# *=*\n':
                 indicator += 1
                 continue
+
             if indicator in read_indicators:
                 profilefile.write(line)
     profilefile.write('# Prometheus initialisation done\n')
     profilefile.write('\n')
 
 
 def define_end(profilefile: io.TextIOWrapper):
@@ -103,15 +104,14 @@
         for line in itertools.islice(read_file, prometheus_initEndSplit, None):
             if line == '# *=*\n':
                 indicator += 1
                 continue
             if indicator in read_indicators:
                 profilefile.write(line)
     profilefile.write('# Prometheus final steps done\n')
-    profilefile.write('\n')
 
 
 def load_df(feather_path: str):
     df = pd.read_feather(feather_path)
     df['Time'] = df['Time'].apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S'))
     time_series = df['Time'].values
     return df, time_series
```

### Comparing `PyProfQueue-0.2.1/PyProfQueue/script.py` & `PyProfQueue-0.2.2/PyProfQueue/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -905,18 +905,31 @@
             profilefile.write('cd ${WORKING_DIR}\n')
             profilefile.write(f'export PYTHON_INSTANCE={sys.executable}')
             profilefile.write('\n')
             if self.profiling is not None:
                 for key in self.profiling.keys():
                     self.initialise_profiling(key, profilefile)
 
+                profilefile.write('export START_TIME=$(date +%s)\n')
+                profilefile.write('sleep 10\n\n')
                 for key in self.profiling.keys():
                     self.run_work_profiling(key, profilefile, bash_options)
-
                 if not self.at_execute:
                     self.run_work(profilefile, bash_options)
-
+                profilefile.write('sleep 10\n')
+                profilefile.write('export END_TIME=$(date +%s)\n')
+                profilefile.write('export DURATION=$((${END_TIME} - ${START_TIME}))\n')
+                profilefile.write('export START=$(date -d @${START_TIME} +"%Y-%m-%d %H:%M:%S")\n')
+                profilefile.write('export END=$(date -d @${END_TIME} +"%Y-%m-%d %H:%M:%S")\n\n')
                 for key in self.profiling.keys():
                     self.end_profiling(key, profilefile)
             else:
+                profilefile.write('export START_TIME=$(date +%s)\n')
+                profilefile.write('sleep 10\n')
                 self.run_work(profilefile, bash_options)
+                profilefile.write('sleep 10\n')
+                profilefile.write('export END_TIME=$(date +%s)\n')
+                profilefile.write('export DURATION=$((${END_TIME} - ${START_TIME}))\n')
+                profilefile.write('export START=$(date -d @${START_TIME} +"%Y-%m-%d %H:%M:%S")\n')
+                profilefile.write('export END=$(date -d @${END_TIME} +"%Y-%m-%d %H:%M:%S")\n\n')
+            profilefile.write("echo 'Run time: '$((${DURATION}/60/60))':'$((${DURATION}/60%60 ))':'$((${DURATION}%60))\n")
         return
```

### Comparing `PyProfQueue-0.2.1/PyProfQueue/submission.py` & `PyProfQueue-0.2.2/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.1/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.2.2/PyProfQueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
 Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.2.1/PyProfQueue.egg-info/SOURCES.txt` & `PyProfQueue-0.2.2/PyProfQueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.1/ReadMe.md` & `PyProfQueue-0.2.2/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.1/setup.py` & `PyProfQueue-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.2.1',
+    version='0.2.2',
     url='https://github.com/uksrc-developers/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md',
```

