# Comparing `tmp/PyProfQueue-0.2.0.tar.gz` & `tmp/PyProfQueue-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.2.0.tar", last modified: Tue May 14 15:11:31 2024, max compression
+gzip compressed data, was "PyProfQueue-0.2.1.tar", last modified: Wed May 22 12:13:03 2024, max compression
```

## Comparing `PyProfQueue-0.2.0.tar` & `PyProfQueue-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    19803 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      350 2024-05-07 13:36:25.000000 PyProfQueue-0.2.0/PyProfQueue/__init__.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    12690 2024-05-07 13:55:56.000000 PyProfQueue-0.2.0/PyProfQueue/plot.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue/profilers/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/__init__.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2340 2024-05-14 14:28:05.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/_template_profiler.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue/profilers/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/_template_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1390 2024-05-14 13:39:52.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      880 2024-05-14 13:39:52.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     3343 2024-05-14 14:33:04.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/likwid.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     3744 2024-05-14 14:28:08.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    38688 2024-05-14 15:10:36.000000 PyProfQueue-0.2.0/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2126 2024-05-09 14:25:46.000000 PyProfQueue-0.2.0/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    19803 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      639 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       56 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    19079 2024-05-14 14:43:03.000000 PyProfQueue-0.2.0/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1355 2024-05-14 14:30:49.000000 PyProfQueue-0.2.0/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.658128 PyProfQueue-0.2.1/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23306 2024-05-22 12:13:03.658128 PyProfQueue-0.2.1/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      404 2024-05-22 12:10:27.000000 PyProfQueue-0.2.1/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue/profilers/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/__init__.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2377 2024-05-14 16:15:39.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/_template_profiler.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue/profilers/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/_template_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1711 2024-05-22 12:01:34.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1643 2024-05-22 12:01:34.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     8023 2024-05-22 11:58:30.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/likwid.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    14926 2024-05-22 11:20:22.000000 PyProfQueue-0.2.1/PyProfQueue/profilers/prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    39177 2024-05-22 11:10:00.000000 PyProfQueue-0.2.1/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2127 2024-05-14 15:39:53.000000 PyProfQueue-0.2.1/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-22 12:13:03.654128 PyProfQueue-0.2.1/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    23306 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      619 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       67 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-22 12:13:03.000000 PyProfQueue-0.2.1/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    22446 2024-05-14 16:16:58.000000 PyProfQueue-0.2.1/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-22 12:13:03.658128 PyProfQueue-0.2.1/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1506 2024-05-22 12:10:27.000000 PyProfQueue-0.2.1/setup.py
```

### Comparing `PyProfQueue-0.2.0/PKG-INFO` & `PyProfQueue-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.0
-Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
-Home-page: https://github.com/Marcus-Keil/PyProfQueue
+Version: 0.2.1
+Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
+Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pytz
 Requires-Dist: pyarrow
+Requires-Dist: matplotlib
 Requires-Dist: promql_http_api==0.3.3
 Requires-Dist: pandas<=2.2.1
 
 # PyProfQueue
 
 ___
 ___
@@ -41,32 +42,24 @@
 ### Script Class
 The *Script* class is used in the following way, and the following options are available:
 ```
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
-                            likwid: bool = False,
-                            likwid_req: list = None,
-                            prometheus: bool = False,
-                            prometheus_ip: str = None, 
-                            prometheus_req: list = None
+                            profiling: dict = None
                             )   
 ```
-|           Option           | Description                                                                                                                                                                     |
-|:--------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-|        queue_system        | The intended target queue system (Supports Slurm and PBS Torque)                                                                                                                |
-|        work_script         | The bash script which contains the queue options and work to be done                                                                                                            |
-|read_queue_system (Optional)| The name of the queue system for which the script was written if it was written for a queue system                                                                              |
-|  queue_options (Optional)  | Any queue options to add or override when compared to the work_script                                                                                                           |
-|     likwid (Optional)      | Bool to determine if likwid should be used. Defaults to False.                                                                                                                  |
-|   likwid_req (Optional)    | Likwid requirements, details can be found in the section about **add_likwid**. Required if likwid Bool is True.                                                                 |
-|   prometheus (Optional)    | Bool to determine if prometheus should be used. Defaults to False.                                                                                                              |
-|  prometheus_ip (Optional)  | IP address of a pre-existing prometheus instance, not providing an address will result in launching a prometheus instance with the address 'http://localhost:9090'              |
-| prometheus_req (Optional)  | Prometheus requirements, details can be found in the section about **add_prometheus**. Required if prometheus Bool is True and no pre-existing prometheus instance is provided. |
+|           Option           | Description                                                                                                                        |
+|:--------------------------:|------------------------------------------------------------------------------------------------------------------------------------|
+|        queue_system        | The intended target queue system (Supports Slurm and PBS Torque)                                                                   |
+|        work_script         | The bash script which contains the queue options and work to be done                                                               |
+|read_queue_system (Optional)| The name of the queue system for which the script was written if it was written for a queue system                                 |
+|  queue_options (Optional)  | Any queue options to add or override when compared to the work_script                                                              |
+|    profiling (Optional)    | Dictionary with keys representing which profiler to use with values of dictionaries listing profiler options such as "requirements"|
 
 
 The options *queue_options* that PyProfQueue currently supports are:
 - 'user'
   - The user ID of the system with which to submit the job (requires admin rights usually)
 - 'nodes'
   - The number of nodes to be requested.
@@ -84,62 +77,15 @@
   - Name of the submitted job.
 - 'workdir'
   - The directory in which the work should be done.
 - 'output'
   - The file, including path, to write the STDOUT to.
 
 Any *Script* object, then comes with three additional methods intended to be used by users. These methods are:
-#### add_likwid
-```
-add_likwid(likwid_req: list)
-```
-- Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
-- This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
-- likwid_req is a list that should contain the necessary lines for the system in use to be able to use liquid. 
 
-For example, loading the likwid module:
-```
-likwid_req = ['module load likwid']
-```
-Example usage of *add_likwid* on a system that has the module environment, but where the likwid module requires the
-oneApi module to be loaded first:
-```
-script.add_likwid(likwid_req=['module load oneApi', 'module load likwid'])
-```
-#### add_prometheus
-```
-add_prometheus(prometheus_req: list, prometheus_ip: str = None)
-```
-- Adds necessary initiation to use measure computing resource usage
-- This can be used if a *Script* object was not initiated with prometheus options, or if they are to be changed
-- prometheus_req is a list that should contain the necessary lines for the system in use to be able to use
-prometheus. The example below shows how to define required environment variable **PROMETHEUS_SOFTWARE**. This variable
-needs to be the path to the prometheus software to be used. This only required if prometheus_ip is not being provided.
-- prometheus_ip is a string which is the ip-address of a pre-existing prometheus instance, if it exists.
-``` 
-prometheus_req = [
-    'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>'
-]
-```
-Example usage of *add_prometheus* where we provide the path to the **PROMETHEUS_SOFTWARE** directory:
-```
-script.add_prometheus(prometheus_req = ['export PROMETHEUS_SOFTWARE=/home/PrometheusSoftware'])
-```
-The **PROMETHEUS_SOFTWARE** directory should have the following structure at minimum, but may contain more files 
-depending on where it was stored and the version of node_exporter and prometheus being used.
-```md
-${PROMETHEUS_SOFTWARE}
-├── node_exporter
-│   └── node_exporter
-└── prometheus
-    ├── prometheus
-    └── prometheus.yml
-```
-Where *node_exporter/node_exporter* is the executable for node_exporter, *prometheus/prometheus* is the executable for 
-prometheus, and *prometheus/prometheus.yml* is the configuration file to be used for prometheus.
 #### change_options
 ```
 change_options(queue_options: dict)
 ```
 - Allows for options to be changed post initiation of a *Script* object, in case the options given in the 
 initialisation are no longer desired.
 
@@ -166,39 +112,102 @@
 |           script            | *Script* object to be submitted to queue                                                                                                                                                                           |
 | tmp_work_script (Optional)  | Desired name of temporary work script. Defaults to "tmp_workfile.sh".                                                                                                                                              |
 |tmp_profile_script (Optional)| Desired name of temporary profile script. Defaults to "tmp_profilefile.sh".                                                                                                                                        |
 |   bash_options (Optional)   | List of options that the user provided bash script may require. Defaults to [' '].                                                                                                                                 |
 |  leave_scripts (Optional)   | Boolean to determine if the temporary scripts should be left or removed after submission. Defaults to True                                                                                                         |
 |       test (Optional)       | Boolean to determine if the script should be submitted, or if the command that would be used should be printed to the terminal. Additionally, this leaves the temporary scripts in tackt so they can be inspected. |
 
-### plot_profiling function
-
-### plot_roof function
+### plot.load_df function
+This function reads the prometheus database created by using prometheus profiling with *PyProfQueue* and stores it 
+into a pandas.DataFrame. This then has the time converted into the format of "yyyy-mm-dd HH:MM:SS" for user readability.
+The times at which datapoints exist are then also given out as a numpy.array on top of returning the dataframe. 
+
+|    Option    | Description                             |
+|:------------:|-----------------------------------------|
+| feather_path | path to the scraped prometheus database |
+### plot.plot_profiling function
+This function plots the results of a prometheus profiling effort. It is compatible with additional features for 
+[Common Workflow Language](https://www.commonwl.org/) (CWL) workflows, if the output from a CWL call is saved to a file.
+
+|            Option            | Description                                                                                                                      |
+|:----------------------------:|----------------------------------------------------------------------------------------------------------------------------------|
+|              df              | pandas.DataFrame of the prometheus profiling data. Obtained from load_df                                                         |
+|         time_series          | numpy.array of the times at which data was collected. Obtained from load_df                                                      |
+|         name_prefix          | Desired path and name prefix for the plots                                                                                       |
+|network_three_mean (Optional) | Boolean on if the network y-limit should be restricted to three times the mean value                                             |
+|     mean_cpu (Optional)      | Boolean on if the mean_cpu usage should be plotted                                                                               |
+|      all_cpu (Optional)      | Boolean on if all cpu usages should be plotted                                                                                   |
+|      memory (Optional)       | Boolean on if the memory usage should be plotted                                                                                 |
+|      network (Optional)      | Boolean on if the network usage should be plotted                                                                                |
+|     cwl_file (Optional)      | Path to a text file containing the ouput of CWL, if it was used to run a workflow. This is used to shade when each step occured. |
+|       label (Optional)       | Boolean to label each CWL step on shaded graphs if cwl_file was provided                                                         |
+|       gant (Optional)        | Boolean on if a gant chart like plot should be created if CWL was used to run a workflow                                         |
+
+### plot.plot_roof function
+This function plots the results of a likwid profiling effort.
+
+|        Option         | Description                                                          |
+|:---------------------:|----------------------------------------------------------------------|
+|      name_prefix      | Desired path and name prefix for the plot                            |
+|        maxperf        | Float of the maximum performance listed in likwid output file        |
+|      maxband          | Float of the maximum memory bandwidth listed in likwid output file   |
+| code_name (Optional)  | String of what to call the code in the legend of the plot            |
+| code_mflop (Optional) | Float of the codes MFLOP/s listed in the likwid output               |
+| code_opint (Optional) | Float of the codes Operational Intensity listed in the likwid output |
 
 ___
 ##  In- and Outputs
 ___
 ### Inputs
 The inputs to the *Script* class and *submit* function have already been described above, what has not been described
 in detail in the input file that users provide. Users must provide the bash script that they wish to profile and submit
 to a queue system. If a bash script with no queue options is provided, then the *read_queue_system* option can be left
 off, or set to None. In this case, unless both *read_queue_system* and *queue_system* are set to None, *queue_options* 
 have to be provided. If queue options are available in the script then *read_queue_system* should be set to the name
 of the queue system that the original script was intended for.
+#### Likwid specific inputs
+In order to use likwid, the key 'likwid' needs to be used in the *profiling* option for the *Script* object. This key 
+then needs to have a value of "requirements" which contains a list of all commands that need to be executed prior to 
+being able to use likwid on the HPC system the script is being submitted to. If, for example, a simple module loading
+is required, it could look like this
+```python
+profiling = {"likwid": {"requirements":["module load likwid"]}}
+```
+#### Prometheus specific inputs
+In order to use prometheus, the key 'prometheus' needs to be used in the *profiling* option for the *Script* object. 
+This key then needs to have a value of "requirements" which has to contain the path to the prometheus instance to use, 
+or it has to contain "ip_address" which then has an IP address, stored as a string, of a pre-existing prometheus
+instance that can be scraped. Here is an example of both, where "<path/to/prometheus>" is used to represent the path
+to the prometheus instance the user would want to use.
+```python
+profiling = {"prometheus": {"requirements":["export PROMETHEUS_SOFTWARE=<path/to/prometheus>"]}}
+# OR
+profiling = {"prometheus": {"ip_address":["127.0.0.1:9090"]}}
+```
+
+#### Both likwid and prometheus
+Here is an example of how the dictionary could look, if both likwid and prometheus were to be used:
+```python
+profiling = {"likwid": {"requirements":["module load likwid"]}, 
+             "prometheus": {"requirements":["export PROMETHEUS_SOFTWARE=<path/to/prometheus>"]}
+             }
+```
 
 ### Outputs
 The output of the *Script* class, is an object that contains all the given options, file paths and other variables 
 needed in order to create the bash scripts that can be submitted to a queue system. The outputs from *submit* 
 depend on the given options. If the *test* and *leave_scripts* are set to **False**, then the output of *submit* is 
 the same as the output of the submission command for the respective queue system being used. If *test* or 
 *leave_scripts* are set to **True** then the output includes two bash scripts. The first contains the original work 
 to be performed, the other contains all the necessary variable declarations and command calls in order to perform 
 the profiling of the given bash script. It is the profiling script that is submitted to the queue. Additionally,
 if *test* is **True**, then the command line will output what command would be used in order to submit the job, but
 the command will not actually be called.
+
+For the plotting functions, the outputs are .png files of each requested plot.
 ___
 ## Example usage
 ___
 Let us look at a toy example to show how this script would be used. Let us assume we have an HPC system that uses slurm.
 This system requires loading the likwid module if we want to use it, and we have downloaded the prometheus codes to the
 directory **/home/Software** and ensured that we can execute both without sudo commands. Let us assume we have the 
 following bash script:
@@ -223,29 +232,28 @@
 submit the script to the queue. We have listed the queue options in the *Script* object initialisation even though it 
 would pull them from the bash script in order to show an example of how they would be listed.
 ```python 
 import PyProfQueue as ppq
 
 ProfileScript = ppq.Script(queue_system='slurm',
                            work_script='./tmp_workfile.sh',
-                           likwid=True,
-                           likwid_req=['module load likwid'],
-                           prometheus=True,
-                           prometheus_req=['export PROMETHEUS_SOFTWARE=/home/Software'],
                            queue_options={
                                'workdir': '/home/queue_work/%x.%j',
                                'account': 'example_project',
                                'cores': '16',
                                'nodes': '1',
                                'output': '/home/queue_work/%x.%j/output.out',
                                'partition': 'example_partition',
                                'name': 'TestSubmission',
                                'tasks': '1',
-                               'time': '00:05:00'
-                           })
+                               'time': '00:05:00'},
+                           profiling={"likwid": {'requirements': ['module load oneAPI_comp/2021.1.0',
+                                                                  'module load likwid/5.2.0']},
+                                      "prometheus": {'requirements': ['export PROMETHEUS_SOFTWARE=/home/Software']}
+                                      })
 
 ppq.submit(ProfileScript, 
            tmp_work_script = './test_workfile.sh',
            tmp_profile_script = './test_profilefile.sh',
            bash_options=['"Hello "', '"World!"'],
            test=True)
 ```
@@ -279,14 +287,15 @@
 ___
 ### Python Requirements
 For the sake of PyProfQueue, the required python version is at least 3.10, as this package utilises the match 
 functionality.
 - numpy
 - pytz
 - pyarrow
+- matplotlib
 - promql_http_api==0.3.3
 - pandas<=2.2.1
 ### Non Python Requirements
 In addition to the python requirements listed above, PyProfQueue also needs to have the following software on the system 
 to which the job will be submitted:
 - [node_exporter](https://prometheus.io/docs/guides/node-exporter/)
 - [prometheus](https://prometheus.io/)
@@ -308,63 +317,90 @@
 
 For the sake of likwid, it needs to be installed or loaded in, in such a way that a user could run the following 
 command without sudo rights:
 ```
 likwid-perfctr -g MEM_DP -f <executable>
 ```
 ___
-## Container Compatibility (If applicable)
+## Container Compatibility
 ___
 This package does not require a container and since it submits to a queue, we do not know how recommended it is to 
 use it from within a container.
 ___
 ## Hardware Requirements
 ___
 As of now, no minimum Hardware requirements are known other than those forced by python 3.10, prometheus, node_exporter
 and likwid.
 ___
 ## Directory Structure
 ___
 ```md
 PyProfQueue
 ├── PyProfQueue
-│   ├── data
-│   │   ├── read_prometheus.py
-│   │   ├── likwid_commands.txt
-│   │   └── prometheus_commands.txt
+│   ├── profilers
+│   │   ├── data
+│   │   │   ├── read_prometheus.py
+│   │   │   ├── _template_commands.txt
+│   │   │   ├── likwid_commands.txt
+│   │   │   └── prometheus_commands.txt
+│   │   ├── __init__.py
+│   │   ├── _template_profiler.py
+│   │   ├── likwid.py
+│   │   └── prometheus.py
 │   ├── __init__.py
 │   ├── plot.py
 │   ├── script.py
 │   └── submission.py
 ├── ReadMe.md
 └── setup.py
 ```
-The directory *PyProfQueue/data* contains a script called *read_prometheus.py* which is used to scrape the prometheus 
-database into a pandas dataframe. It also includes the two text files, *likwid_commands.txt* and 
-*prometheus_commands.txt*, which list the bash commands needed to initialise and end likwid and prometheus respectively.
+The directory *PyProfQueue/PyProfQueue* contains the *plot.py*. *script.py* and *submission.py* scripts which contain the 
+definition of the plotting functions, *Script* class and *submission()* function respectively.
+
+The directory *PyProfQueue/PyProfQueue/profilers* contains scripts of the individual profilers that PyProfQueue is 
+compatible with including a template version that can be used to add additional profiling software compatibility to 
+PyProfQueue. *PyProfQueue/PyProfQueue/profilers/data* contains a script called *read_prometheus.py* which is used to 
+scrape the prometheus database into a pandas dataframe. It also includes the text files that list the bash commands 
+needed to initialise run and end profiling software, as well as a template version for adding more profiling software 
+compatibility.
+
 
-The directory *PyProfQueue/PyProfQueue* contains the *script.py* and *submission.py* scripts which contain the 
-definition of the *Script* class and *submission()* function respectively.
 
 The base directory contains the ReadMe.md file, and the setup.py file so that the package can be installed.
 ___
 ## Adding new Queue systems
 ___
 A future goal for development on PyProfQueue is to add additional queue suport beyond slurm and torque. In order to add 
 new queue system compatibility refer to the block comments in the *Script* class in script.py. Each of the four section 
 that needs changes is marked with "Queue System specifics" followed by a {1}, {2}, {3} or {4}.
 ___
+## Adding new Profiling software
+___
+In order to add new profiling software compatibility, a new script would need to be added to the 
+*PyProfQueue/PyProfQueue/profilers* directory. This script would need to have the name of how the specific profiler
+should be called, as well as the following two functions:
+- define_initialise(profilefile: io.TextIOWrapper, profilerdict: dict = None)
+- define_end(profilefile: io.TextIOWrapper)
+
+Both of these functions can read from a .txt file, which can be stored in *PyProfQueue/PyProfQueue/profilers/data*.
+The first *define_initialise* is there to add any variable declarations or code to the profiling bash script that would
+be needed in order to run the profiler. The second is any calls needed in order to terminate, or collect data post 
+running the profiler.
+
+If the profiler being added needs to be used in order to execute the user provided bash script, then the function 
+*define_run(profilefile: io.TextIOWrapper, bash_options: list, tmp_work_script: str)* should be defined in the 
+script for the specific profiler. This function should write the needed command to use the profilerto the profiling 
+file.
+___
 ___
 
 
 # To Do
 ___
 ___
-- Add in comments to describe all functions and improve readability of code
-- Reformat the location of the profiling functions to make adding more, easier
 - Update the package format to follow more modern conventions for installing requirements
   - e.g. add pyproject.toml 
 - Add Vtune profiling support
 - Add Linaro Forge profiling support
 ___
 ___
 # UKSRC related Links
```

### Comparing `PyProfQueue-0.2.0/PyProfQueue/plot.py` & `PyProfQueue-0.2.1/PyProfQueue/profilers/prometheus.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,118 @@
 from datetime import datetime, timedelta
 from matplotlib.pyplot import cm
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdt
-# import matplotlib as mpl
 import pandas as pd
 import numpy as np
 import pytz
 
+from importlib import resources as impresources
+import itertools
+import io
+
+from . import data
+
 alpha = 0.75
 DPI = 100
 avg_xSize, avg_ySize = 50, 10
 MeanMult = 3
 LegCols = 7
 
-
 tz = pytz.timezone('UTC')
 
+prometheus_file_path = impresources.files(data) / "prometheus_commands.txt"
+prometheus_initEndSplit = -1
+IP_address = None
+
+
+def define_initialise(profilefile: io.TextIOWrapper, profilerdict: dict = None):
+    '''
+    define_initialise creates any needed variables, and writes the required arguments into the profile_file in order
+    to initialise the profiling for a user, in this case that is <template_profiler>.
+
+    Parameters
+    ----------
+    profilefile: io.TextIOWrapper = Open text file that can be written to and is being used to initiate, call and
+        terminate all profiling codes that are to be executed with the user specified bash script.
+    profilerdict: dict = dictionary containing required arguments that prometheus has or a preexisting ip_address for
+        a prometheus instance.
+    Returns
+    -------
+    None
+    '''
+    global prometheus_file_path
+    global prometheus_initEndSplit
+    global IP_address
+    if 'ip_address' not in profilerdict.keys() and 'requirements' not in profilerdict.keys():
+        exit("Must provide prometheus requirements list, or existing prometheus IP address, neither was given.")
+    profilefile.write('# Prometheus initialisation declarations\n')
+    if 'ip_address' not in profilerdict.keys():
+        profilefile.write("export PROMETHEUS_IP=http://localhost:9090\n")
+        for i in profilerdict['requirements']:
+            profilefile.write(i)
+            profilefile.write('\n')
+    else:
+        IP_address = profilerdict['ip_address']
+        profilefile.write(f"export PROMETHEUS_IP={IP_address}\n")
+    profilefile.write('export PROMETHEUS_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
+    scrape_path = str(impresources.path(data, 'read_prometheus.py'))[:-19]
+    profilefile.write('export PROFILE_SCRAPE={}\n'.format(scrape_path))
+    profilefile.write('\n')
+    final_init_indicator = 2
+    if IP_address is None:
+        read_indicators = [0, 1, 2]
+    else:
+        read_indicators = [0, 2]
+    indicator = 0
+    with open(prometheus_file_path, 'r') as read_file:
+        for number, line in enumerate(read_file):
+            if line == '# *=*\n' and indicator >= final_init_indicator:
+                prometheus_initEndSplit = number + 1
+                break
+            elif line == '# *=*\n':
+                indicator += 1
+                continue
+            if indicator in read_indicators:
+                profilefile.write(line)
+    profilefile.write('# Prometheus initialisation done\n')
+    profilefile.write('\n')
+
+
+def define_end(profilefile: io.TextIOWrapper):
+    '''
+    define_end terminates and scrapes any data from the profiler that was used to profile the user specified bash
+    script, in this case that is <template_profiler>.
+    Parameters
+    ----------
+    profilefile: io.TextIOWrapper = Open text file that can be written to and is being used to initiate, call and
+        terminate all profiling codes that are to be executed with the user specified bash script.
+
+    Returns
+    -------
+    None
+    '''
+    global prometheus_file_path
+    global prometheus_initEndSplit
+    profilefile.write('# Prometheus final steps declarations\n')
+    if IP_address is None:
+        read_indicators = [0, 1, 2]
+    else:
+        read_indicators = [0, 2]
+    indicator = 0
+    with open(prometheus_file_path, 'r') as read_file:
+        for line in itertools.islice(read_file, prometheus_initEndSplit, None):
+            if line == '# *=*\n':
+                indicator += 1
+                continue
+            if indicator in read_indicators:
+                profilefile.write(line)
+    profilefile.write('# Prometheus final steps done\n')
+    profilefile.write('\n')
+
 
 def load_df(feather_path: str):
     df = pd.read_feather(feather_path)
     df['Time'] = df['Time'].apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S'))
     time_series = df['Time'].values
     return df, time_series
 
@@ -73,25 +166,25 @@
             h = next(hatch)
         except:
             hatch = iter(['/', '|', '-', '+', 'x', 'O', '*'])
             h = next(hatch)
         plt.vlines(row['Start'], 0, 100, colors=c, linestyle='--')
         plt.vlines(row['End'], 0, 100, colors=c, linestyle='--')
         if label:
-            plt.axvspan(row['Start'], row['End'] + timedelta(seconds=10), 0,100,
+            plt.axvspan(row['Start'], row['End'] + timedelta(seconds=10), 0, 100,
                         alpha=alpha, color=c, label=row['Step'], linestyle='--', hatch=h)
         else:
-            plt.axvspan(row['Start'], row['End'] + timedelta(seconds=10), 0,100,
+            plt.axvspan(row['Start'], row['End'] + timedelta(seconds=10), 0, 100,
                         alpha=alpha, color=c, linestyle='--', hatch=h)
 
 
-def plot_profiling(df: pd.DataFrame, time_series: np.array, name_prefix: str, 
-                   cwl_file: str = None, label: bool = True, network_three_mean: bool = True,
-                   mean_cpu: bool = True, all_cpu: bool = True, memory: bool = True, 
-                   network: bool = True, gant: bool = True):
+def plot_prom_profiling(df: pd.DataFrame, time_series: np.array, name_prefix: str,
+                        cwl_file: str = None, label: bool = True, network_three_mean: bool = True,
+                        mean_cpu: bool = True, all_cpu: bool = True, memory: bool = True,
+                        network: bool = True, gant: bool = True):
     if cwl_file is not None:
         df_steps = cwl_pass(cwl_file)
     # Mean CPU
     if mean_cpu:
         MeanCPU_figure = plt.figure(figsize=(avg_xSize, avg_ySize))
         MeanCPU_figure.suptitle("Mean CPU usage (Percentage)", fontsize=20)
         plt.gca().xaxis.set_major_formatter(mdt.DateFormatter('%y-%m-%d %T'))
@@ -121,15 +214,15 @@
     if all_cpu:
         N_Cores = len(df.filter(like='CPU Usage:').columns)
         sub_xSize, sub_ySize = 20, 15
         N_rows = 8
         N_columns = int(N_Cores / N_rows)
         Yscaling = 0.95
         Xscaling = 0.99
-        
+
         AllCPU = plt.figure(figsize=(sub_xSize, sub_ySize))
         AllCPU.suptitle("Individual CPU usage (Percentage)", fontsize=20)
         cpuNumber = np.array([int(x[-2:]) for x in df.filter(like='CPU Usage:').columns.array])
         Usage_columns = df.filter(like='CPU Usage:').columns.array
         sorted_columns = np.array([x for _, x in sorted(zip(cpuNumber, Usage_columns))])
         for i, cpuUsage in enumerate(sorted_columns):
             row, col = np.abs((i // N_columns) - N_rows), i % N_columns
@@ -150,15 +243,15 @@
             ax.set_ylim([0, 105])
             ax.set_xlim([time_series[0], time_series[-1]])
             ax.yaxis.set_visible(False)
             ax.xaxis.set_visible(False)
             # ax.locator_params(axis='x', nbins=4)
         plt.savefig(name_prefix + '_AllCPU_Usages.png', bbox_inches='tight', dpi=DPI)
     # Memory Plots
-    if memory: 
+    if memory:
         memory_figure = plt.figure(figsize=(avg_xSize, avg_ySize))
         memory_figure.suptitle("RAM usage [GB]", fontsize=20)
         plt.gca().xaxis.set_major_formatter(mdt.DateFormatter('%y-%m-%d %T'))
         if cwl_file is not None:
             plot_shades(df_steps, label)
         plt.fill_between(time_series, df['Memory Usage [GB]'], 0, label="RAM usage [GB]", linestyle='-', alpha=alpha)
         plt.legend(ncol=LegCols, prop={'size': 20}, framealpha=1, bbox_to_anchor=(0.96, -0.1))
@@ -166,15 +259,15 @@
         plt.xlim([time_series[0], time_series[-1]])
         plt.xlabel("Time", fontsize=20)
         plt.xticks(fontsize=20)
         plt.ylabel("RAM usage [GB]", fontsize=20)
         plt.yticks(fontsize=20)
         plt.savefig(name_prefix + '_Memory_Usage.png', bbox_inches='tight', dpi=DPI)
     # Network Plots
-    if network: 
+    if network:
         network_figure = plt.figure(figsize=(avg_xSize, avg_ySize))
         network_figure.suptitle("Network usage [Received positive, Sent negative KB]", fontsize=20)
         plt.gca().xaxis.set_major_formatter(mdt.DateFormatter('%y-%m-%d %T'))
         if cwl_file is not None:
             plot_shades(df_steps, label)
         maxY = 0
         minY = 0
@@ -211,47 +304,8 @@
                  left=mdt.date2num(df_steps['Start']), color=df_steps['Status'])
         plt.xlabel("Time", fontsize=20)
         plt.xticks(fontsize=20)
         plt.xlim([time_series[0], time_series[-1]])
         plt.ylabel("Step", fontsize=20)
         plt.yticks(fontsize=20)
         plt.savefig(name_prefix + '_StepGant.png', bbox_inches='tight', dpi=DPI)
-    return
-
-
-def plot_roof(name_prefix: str, maxperf: float, maxband: float,
-              code_name: str = 'code', code_mflop: float = None, code_opint: float = None):
-    if code_mflop is not None:
-        if code_opint * maxband < maxperf:
-            Percentage = int((code_mflop / (code_opint * maxband)) * 100)
-        else:
-            Percentage = int((code_mflop / maxperf) * 100)
-        Dot = True
-    else:
-        Dot = False
-
-    if maxperf / maxband > 1:
-        maxX = (maxperf / maxband) * 2
-        if Dot:
-            if (maxX < code_opint):
-                maxX = code_opint
-    else:
-        maxX = 1
-        if Dot:
-            if (maxX < code_opint):
-                maxX = code_opint
-
-    x_Axis = np.append(np.linspace(0, maxperf / maxband, 10), maxX)
-    y = np.array([x * maxband if ((x * maxband) < maxperf) else maxperf for x in x_Axis])
-    Roofline = plt.figure(figsize=(10, 7))
-    Roofline.suptitle("Roofline Model", fontsize=20)
-    plt.plot(x_Axis, y, label="Roofline")
-    plt.vlines(maxperf / maxband, 0, maxperf, linestyle='--', color='gray', alpha=0.5,
-               label='Bandwidth to CPU limit boarder')
-    plt.xlabel("Operational Intensity")
-    plt.ylabel("Performance [MFLOP/s]")
-    if Dot:
-        plt.plot(code_opint, code_mflop, 'ro', label=f'{code_name} Performance [~{Percentage}% of roofline]')
-        plt.xlim([0, x_Axis.max()])
-    plt.ylim([0, maxperf * 1.1])
-    plt.legend(loc='upper left')
-    plt.savefig(name_prefix + '_Roofline.png', bbox_inches='tight')
+    return
```

### Comparing `PyProfQueue-0.2.0/PyProfQueue/profilers/_template_profiler.py` & `PyProfQueue-0.2.1/PyProfQueue/profilers/_template_profiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Returns
     -------
     None
     '''
     print('Template Function')
     return
 
-def define_run(profilefile, bash_options=[''], tmp_work_script: str = './tmp_workfile.sh'):
+def define_run(profilefile: io.TextIOWrapper, bash_options: list, tmp_work_script: str = './tmp_workfile.sh'):
     '''
     define_run calls the user given bash script using <template_profiler> to execute and profile the work done.
     Parameters. This only has to be defined, if the profiler in question is used to execute the user given bash script.
     ----------
     profilefile: io.TextIOWrapper = Open text file that can be written to and is being used to initiate, call and
         terminate all profiling codes that are to be executed with the user specified bash script.
     bash_options: list = List of bash options that the user specified bash script needs to execute as intended
@@ -40,15 +40,15 @@
     -------
     None
     '''
     print('Template Function')
     return
 
 
-def define_end(profilefile):
+def define_end(profilefile: io.TextIOWrapper):
     '''
     define_end terminates and scrapes any data from the profiler that was used to profile the user specified bash
     script, in this case that is <template_profiler>.
     Parameters
     ----------
     profilefile: io.TextIOWrapper = Open text file that can be written to and is being used to initiate, call and
         terminate all profiling codes that are to be executed with the user specified bash script.
```

### Comparing `PyProfQueue-0.2.0/PyProfQueue/profilers/data/read_prometheus.py` & `PyProfQueue-0.2.1/PyProfQueue/profilers/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.2.0/PyProfQueue/script.py` & `PyProfQueue-0.2.1/PyProfQueue/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # Built in Modules
 import importlib
-import itertools
 import sys
-# Local package imports
-
-# from . import profilers
 
 
 class Script:
     """
     Class to read existing bash scripts, pull out the options and create an object that contains all the
     queue options, bash options, and desired profiling methods to be injected
 
@@ -206,14 +202,35 @@
                 current_prof.define_run(profilefile=profilefile,
                                         bash_options=bash_options,
                                         tmp_work_script=self.tmp_work_script)
                 self.at_execute = True
             else:
                 exit(f"Multiple at execution profilers were defined. Failed when adding profiler {profiler}")
 
+    def run_work(self, profilefile, bash_options=['']):
+        """
+        run_work_profiling writes into the profile bash script the call to run the user defined bash script. This is
+        used when no profiler needs to execute the user defined bash script.
+
+        Parameters
+        ----------
+        profilefile: io.TextIOWrapper
+            open profile file with write permissions.
+        bash_options: list
+            List of bash options to pass to the user defined bash script.
+
+        Returns
+        -------
+
+        """
+        profilefile.write('bash {} {}\n'.format(self.tmp_work_script,
+                                                ' '.join(str(x) for x in bash_options)))
+        profilefile.write('\n')
+        return
+
     def end_profiling(self, profiler, profilefile):
         """
         end_profiling is used to call the define_end() function of the different profilers.
 
         Parameters
         ----------
         profiler: str
@@ -824,15 +841,14 @@
         """
         with open(self.tmp_work_script, 'w') as workfile:
             workfile.seek(0)
             for line in self.works:
                 workfile.write(line)
         return
 
-
     def add_options(self, profilefile):
         """
         add_options adds the queue options from the Script object to the profile file.
         Parameters
         ----------
         profilefile: io.TextIOWrapper
             open profile file with write access.
@@ -883,14 +899,15 @@
                 self.add_options(profilefile)
 
             profilefile.write('export WORKING_DIR={}\n'.format(self.work_dir))
             profilefile.write('if [ ! -d  "${WORKING_DIR}" ]; then\n')
             profilefile.write('  mkdir ${WORKING_DIR}\n')
             profilefile.write('fi\n')
             profilefile.write('cd ${WORKING_DIR}\n')
+            profilefile.write(f'export PYTHON_INSTANCE={sys.executable}')
             profilefile.write('\n')
             if self.profiling is not None:
                 for key in self.profiling.keys():
                     self.initialise_profiling(key, profilefile)
 
                 for key in self.profiling.keys():
                     self.run_work_profiling(key, profilefile, bash_options)
@@ -899,13 +916,7 @@
                     self.run_work(profilefile, bash_options)
 
                 for key in self.profiling.keys():
                     self.end_profiling(key, profilefile)
             else:
                 self.run_work(profilefile, bash_options)
         return
-
-    def run_work(self, profilefile, bash_options=['']):
-        profilefile.write('bash {} {}\n'.format(self.tmp_work_script,
-                                                ' '.join(str(x) for x in bash_options)))
-        profilefile.write('\n')
-        return
```

### Comparing `PyProfQueue-0.2.0/PyProfQueue/submission.py` & `PyProfQueue-0.2.1/PyProfQueue/submission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Built in Modules
 import subprocess
 import time
+
 # Local package imports
 from .script import Script
 
 
 def submit(script: Script,
            tmp_work_script: str = './tmp_workfile.sh',
            tmp_profile_script: str = './tmp_profilefile.sh',
```

### Comparing `PyProfQueue-0.2.0/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.2.1/PyProfQueue.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.2.0
-Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
-Home-page: https://github.com/Marcus-Keil/PyProfQueue
+Version: 0.2.1
+Summary: PyProfQueue serves as a python package that can take in existing bash scripts, add prometheus monitoring calls and likwid performance measure calls, and submit the script to an HPC queue system on the users' behalf.
+Home-page: https://github.com/uksrc-developers/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pytz
 Requires-Dist: pyarrow
+Requires-Dist: matplotlib
 Requires-Dist: promql_http_api==0.3.3
 Requires-Dist: pandas<=2.2.1
 
 # PyProfQueue
 
 ___
 ___
@@ -41,32 +42,24 @@
 ### Script Class
 The *Script* class is used in the following way, and the following options are available:
 ```
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
-                            likwid: bool = False,
-                            likwid_req: list = None,
-                            prometheus: bool = False,
-                            prometheus_ip: str = None, 
-                            prometheus_req: list = None
+                            profiling: dict = None
                             )   
 ```
-|           Option           | Description                                                                                                                                                                     |
-|:--------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-|        queue_system        | The intended target queue system (Supports Slurm and PBS Torque)                                                                                                                |
-|        work_script         | The bash script which contains the queue options and work to be done                                                                                                            |
-|read_queue_system (Optional)| The name of the queue system for which the script was written if it was written for a queue system                                                                              |
-|  queue_options (Optional)  | Any queue options to add or override when compared to the work_script                                                                                                           |
-|     likwid (Optional)      | Bool to determine if likwid should be used. Defaults to False.                                                                                                                  |
-|   likwid_req (Optional)    | Likwid requirements, details can be found in the section about **add_likwid**. Required if likwid Bool is True.                                                                 |
-|   prometheus (Optional)    | Bool to determine if prometheus should be used. Defaults to False.                                                                                                              |
-|  prometheus_ip (Optional)  | IP address of a pre-existing prometheus instance, not providing an address will result in launching a prometheus instance with the address 'http://localhost:9090'              |
-| prometheus_req (Optional)  | Prometheus requirements, details can be found in the section about **add_prometheus**. Required if prometheus Bool is True and no pre-existing prometheus instance is provided. |
+|           Option           | Description                                                                                                                        |
+|:--------------------------:|------------------------------------------------------------------------------------------------------------------------------------|
+|        queue_system        | The intended target queue system (Supports Slurm and PBS Torque)                                                                   |
+|        work_script         | The bash script which contains the queue options and work to be done                                                               |
+|read_queue_system (Optional)| The name of the queue system for which the script was written if it was written for a queue system                                 |
+|  queue_options (Optional)  | Any queue options to add or override when compared to the work_script                                                              |
+|    profiling (Optional)    | Dictionary with keys representing which profiler to use with values of dictionaries listing profiler options such as "requirements"|
 
 
 The options *queue_options* that PyProfQueue currently supports are:
 - 'user'
   - The user ID of the system with which to submit the job (requires admin rights usually)
 - 'nodes'
   - The number of nodes to be requested.
@@ -84,62 +77,15 @@
   - Name of the submitted job.
 - 'workdir'
   - The directory in which the work should be done.
 - 'output'
   - The file, including path, to write the STDOUT to.
 
 Any *Script* object, then comes with three additional methods intended to be used by users. These methods are:
-#### add_likwid
-```
-add_likwid(likwid_req: list)
-```
-- Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
-- This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
-- likwid_req is a list that should contain the necessary lines for the system in use to be able to use liquid. 
 
-For example, loading the likwid module:
-```
-likwid_req = ['module load likwid']
-```
-Example usage of *add_likwid* on a system that has the module environment, but where the likwid module requires the
-oneApi module to be loaded first:
-```
-script.add_likwid(likwid_req=['module load oneApi', 'module load likwid'])
-```
-#### add_prometheus
-```
-add_prometheus(prometheus_req: list, prometheus_ip: str = None)
-```
-- Adds necessary initiation to use measure computing resource usage
-- This can be used if a *Script* object was not initiated with prometheus options, or if they are to be changed
-- prometheus_req is a list that should contain the necessary lines for the system in use to be able to use
-prometheus. The example below shows how to define required environment variable **PROMETHEUS_SOFTWARE**. This variable
-needs to be the path to the prometheus software to be used. This only required if prometheus_ip is not being provided.
-- prometheus_ip is a string which is the ip-address of a pre-existing prometheus instance, if it exists.
-``` 
-prometheus_req = [
-    'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>'
-]
-```
-Example usage of *add_prometheus* where we provide the path to the **PROMETHEUS_SOFTWARE** directory:
-```
-script.add_prometheus(prometheus_req = ['export PROMETHEUS_SOFTWARE=/home/PrometheusSoftware'])
-```
-The **PROMETHEUS_SOFTWARE** directory should have the following structure at minimum, but may contain more files 
-depending on where it was stored and the version of node_exporter and prometheus being used.
-```md
-${PROMETHEUS_SOFTWARE}
-├── node_exporter
-│   └── node_exporter
-└── prometheus
-    ├── prometheus
-    └── prometheus.yml
-```
-Where *node_exporter/node_exporter* is the executable for node_exporter, *prometheus/prometheus* is the executable for 
-prometheus, and *prometheus/prometheus.yml* is the configuration file to be used for prometheus.
 #### change_options
 ```
 change_options(queue_options: dict)
 ```
 - Allows for options to be changed post initiation of a *Script* object, in case the options given in the 
 initialisation are no longer desired.
 
@@ -166,39 +112,102 @@
 |           script            | *Script* object to be submitted to queue                                                                                                                                                                           |
 | tmp_work_script (Optional)  | Desired name of temporary work script. Defaults to "tmp_workfile.sh".                                                                                                                                              |
 |tmp_profile_script (Optional)| Desired name of temporary profile script. Defaults to "tmp_profilefile.sh".                                                                                                                                        |
 |   bash_options (Optional)   | List of options that the user provided bash script may require. Defaults to [' '].                                                                                                                                 |
 |  leave_scripts (Optional)   | Boolean to determine if the temporary scripts should be left or removed after submission. Defaults to True                                                                                                         |
 |       test (Optional)       | Boolean to determine if the script should be submitted, or if the command that would be used should be printed to the terminal. Additionally, this leaves the temporary scripts in tackt so they can be inspected. |
 
-### plot_profiling function
-
-### plot_roof function
+### plot.load_df function
+This function reads the prometheus database created by using prometheus profiling with *PyProfQueue* and stores it 
+into a pandas.DataFrame. This then has the time converted into the format of "yyyy-mm-dd HH:MM:SS" for user readability.
+The times at which datapoints exist are then also given out as a numpy.array on top of returning the dataframe. 
+
+|    Option    | Description                             |
+|:------------:|-----------------------------------------|
+| feather_path | path to the scraped prometheus database |
+### plot.plot_profiling function
+This function plots the results of a prometheus profiling effort. It is compatible with additional features for 
+[Common Workflow Language](https://www.commonwl.org/) (CWL) workflows, if the output from a CWL call is saved to a file.
+
+|            Option            | Description                                                                                                                      |
+|:----------------------------:|----------------------------------------------------------------------------------------------------------------------------------|
+|              df              | pandas.DataFrame of the prometheus profiling data. Obtained from load_df                                                         |
+|         time_series          | numpy.array of the times at which data was collected. Obtained from load_df                                                      |
+|         name_prefix          | Desired path and name prefix for the plots                                                                                       |
+|network_three_mean (Optional) | Boolean on if the network y-limit should be restricted to three times the mean value                                             |
+|     mean_cpu (Optional)      | Boolean on if the mean_cpu usage should be plotted                                                                               |
+|      all_cpu (Optional)      | Boolean on if all cpu usages should be plotted                                                                                   |
+|      memory (Optional)       | Boolean on if the memory usage should be plotted                                                                                 |
+|      network (Optional)      | Boolean on if the network usage should be plotted                                                                                |
+|     cwl_file (Optional)      | Path to a text file containing the ouput of CWL, if it was used to run a workflow. This is used to shade when each step occured. |
+|       label (Optional)       | Boolean to label each CWL step on shaded graphs if cwl_file was provided                                                         |
+|       gant (Optional)        | Boolean on if a gant chart like plot should be created if CWL was used to run a workflow                                         |
+
+### plot.plot_roof function
+This function plots the results of a likwid profiling effort.
+
+|        Option         | Description                                                          |
+|:---------------------:|----------------------------------------------------------------------|
+|      name_prefix      | Desired path and name prefix for the plot                            |
+|        maxperf        | Float of the maximum performance listed in likwid output file        |
+|      maxband          | Float of the maximum memory bandwidth listed in likwid output file   |
+| code_name (Optional)  | String of what to call the code in the legend of the plot            |
+| code_mflop (Optional) | Float of the codes MFLOP/s listed in the likwid output               |
+| code_opint (Optional) | Float of the codes Operational Intensity listed in the likwid output |
 
 ___
 ##  In- and Outputs
 ___
 ### Inputs
 The inputs to the *Script* class and *submit* function have already been described above, what has not been described
 in detail in the input file that users provide. Users must provide the bash script that they wish to profile and submit
 to a queue system. If a bash script with no queue options is provided, then the *read_queue_system* option can be left
 off, or set to None. In this case, unless both *read_queue_system* and *queue_system* are set to None, *queue_options* 
 have to be provided. If queue options are available in the script then *read_queue_system* should be set to the name
 of the queue system that the original script was intended for.
+#### Likwid specific inputs
+In order to use likwid, the key 'likwid' needs to be used in the *profiling* option for the *Script* object. This key 
+then needs to have a value of "requirements" which contains a list of all commands that need to be executed prior to 
+being able to use likwid on the HPC system the script is being submitted to. If, for example, a simple module loading
+is required, it could look like this
+```python
+profiling = {"likwid": {"requirements":["module load likwid"]}}
+```
+#### Prometheus specific inputs
+In order to use prometheus, the key 'prometheus' needs to be used in the *profiling* option for the *Script* object. 
+This key then needs to have a value of "requirements" which has to contain the path to the prometheus instance to use, 
+or it has to contain "ip_address" which then has an IP address, stored as a string, of a pre-existing prometheus
+instance that can be scraped. Here is an example of both, where "<path/to/prometheus>" is used to represent the path
+to the prometheus instance the user would want to use.
+```python
+profiling = {"prometheus": {"requirements":["export PROMETHEUS_SOFTWARE=<path/to/prometheus>"]}}
+# OR
+profiling = {"prometheus": {"ip_address":["127.0.0.1:9090"]}}
+```
+
+#### Both likwid and prometheus
+Here is an example of how the dictionary could look, if both likwid and prometheus were to be used:
+```python
+profiling = {"likwid": {"requirements":["module load likwid"]}, 
+             "prometheus": {"requirements":["export PROMETHEUS_SOFTWARE=<path/to/prometheus>"]}
+             }
+```
 
 ### Outputs
 The output of the *Script* class, is an object that contains all the given options, file paths and other variables 
 needed in order to create the bash scripts that can be submitted to a queue system. The outputs from *submit* 
 depend on the given options. If the *test* and *leave_scripts* are set to **False**, then the output of *submit* is 
 the same as the output of the submission command for the respective queue system being used. If *test* or 
 *leave_scripts* are set to **True** then the output includes two bash scripts. The first contains the original work 
 to be performed, the other contains all the necessary variable declarations and command calls in order to perform 
 the profiling of the given bash script. It is the profiling script that is submitted to the queue. Additionally,
 if *test* is **True**, then the command line will output what command would be used in order to submit the job, but
 the command will not actually be called.
+
+For the plotting functions, the outputs are .png files of each requested plot.
 ___
 ## Example usage
 ___
 Let us look at a toy example to show how this script would be used. Let us assume we have an HPC system that uses slurm.
 This system requires loading the likwid module if we want to use it, and we have downloaded the prometheus codes to the
 directory **/home/Software** and ensured that we can execute both without sudo commands. Let us assume we have the 
 following bash script:
@@ -223,29 +232,28 @@
 submit the script to the queue. We have listed the queue options in the *Script* object initialisation even though it 
 would pull them from the bash script in order to show an example of how they would be listed.
 ```python 
 import PyProfQueue as ppq
 
 ProfileScript = ppq.Script(queue_system='slurm',
                            work_script='./tmp_workfile.sh',
-                           likwid=True,
-                           likwid_req=['module load likwid'],
-                           prometheus=True,
-                           prometheus_req=['export PROMETHEUS_SOFTWARE=/home/Software'],
                            queue_options={
                                'workdir': '/home/queue_work/%x.%j',
                                'account': 'example_project',
                                'cores': '16',
                                'nodes': '1',
                                'output': '/home/queue_work/%x.%j/output.out',
                                'partition': 'example_partition',
                                'name': 'TestSubmission',
                                'tasks': '1',
-                               'time': '00:05:00'
-                           })
+                               'time': '00:05:00'},
+                           profiling={"likwid": {'requirements': ['module load oneAPI_comp/2021.1.0',
+                                                                  'module load likwid/5.2.0']},
+                                      "prometheus": {'requirements': ['export PROMETHEUS_SOFTWARE=/home/Software']}
+                                      })
 
 ppq.submit(ProfileScript, 
            tmp_work_script = './test_workfile.sh',
            tmp_profile_script = './test_profilefile.sh',
            bash_options=['"Hello "', '"World!"'],
            test=True)
 ```
@@ -279,14 +287,15 @@
 ___
 ### Python Requirements
 For the sake of PyProfQueue, the required python version is at least 3.10, as this package utilises the match 
 functionality.
 - numpy
 - pytz
 - pyarrow
+- matplotlib
 - promql_http_api==0.3.3
 - pandas<=2.2.1
 ### Non Python Requirements
 In addition to the python requirements listed above, PyProfQueue also needs to have the following software on the system 
 to which the job will be submitted:
 - [node_exporter](https://prometheus.io/docs/guides/node-exporter/)
 - [prometheus](https://prometheus.io/)
@@ -308,63 +317,90 @@
 
 For the sake of likwid, it needs to be installed or loaded in, in such a way that a user could run the following 
 command without sudo rights:
 ```
 likwid-perfctr -g MEM_DP -f <executable>
 ```
 ___
-## Container Compatibility (If applicable)
+## Container Compatibility
 ___
 This package does not require a container and since it submits to a queue, we do not know how recommended it is to 
 use it from within a container.
 ___
 ## Hardware Requirements
 ___
 As of now, no minimum Hardware requirements are known other than those forced by python 3.10, prometheus, node_exporter
 and likwid.
 ___
 ## Directory Structure
 ___
 ```md
 PyProfQueue
 ├── PyProfQueue
-│   ├── data
-│   │   ├── read_prometheus.py
-│   │   ├── likwid_commands.txt
-│   │   └── prometheus_commands.txt
+│   ├── profilers
+│   │   ├── data
+│   │   │   ├── read_prometheus.py
+│   │   │   ├── _template_commands.txt
+│   │   │   ├── likwid_commands.txt
+│   │   │   └── prometheus_commands.txt
+│   │   ├── __init__.py
+│   │   ├── _template_profiler.py
+│   │   ├── likwid.py
+│   │   └── prometheus.py
 │   ├── __init__.py
 │   ├── plot.py
 │   ├── script.py
 │   └── submission.py
 ├── ReadMe.md
 └── setup.py
 ```
-The directory *PyProfQueue/data* contains a script called *read_prometheus.py* which is used to scrape the prometheus 
-database into a pandas dataframe. It also includes the two text files, *likwid_commands.txt* and 
-*prometheus_commands.txt*, which list the bash commands needed to initialise and end likwid and prometheus respectively.
+The directory *PyProfQueue/PyProfQueue* contains the *plot.py*. *script.py* and *submission.py* scripts which contain the 
+definition of the plotting functions, *Script* class and *submission()* function respectively.
+
+The directory *PyProfQueue/PyProfQueue/profilers* contains scripts of the individual profilers that PyProfQueue is 
+compatible with including a template version that can be used to add additional profiling software compatibility to 
+PyProfQueue. *PyProfQueue/PyProfQueue/profilers/data* contains a script called *read_prometheus.py* which is used to 
+scrape the prometheus database into a pandas dataframe. It also includes the text files that list the bash commands 
+needed to initialise run and end profiling software, as well as a template version for adding more profiling software 
+compatibility.
+
 
-The directory *PyProfQueue/PyProfQueue* contains the *script.py* and *submission.py* scripts which contain the 
-definition of the *Script* class and *submission()* function respectively.
 
 The base directory contains the ReadMe.md file, and the setup.py file so that the package can be installed.
 ___
 ## Adding new Queue systems
 ___
 A future goal for development on PyProfQueue is to add additional queue suport beyond slurm and torque. In order to add 
 new queue system compatibility refer to the block comments in the *Script* class in script.py. Each of the four section 
 that needs changes is marked with "Queue System specifics" followed by a {1}, {2}, {3} or {4}.
 ___
+## Adding new Profiling software
+___
+In order to add new profiling software compatibility, a new script would need to be added to the 
+*PyProfQueue/PyProfQueue/profilers* directory. This script would need to have the name of how the specific profiler
+should be called, as well as the following two functions:
+- define_initialise(profilefile: io.TextIOWrapper, profilerdict: dict = None)
+- define_end(profilefile: io.TextIOWrapper)
+
+Both of these functions can read from a .txt file, which can be stored in *PyProfQueue/PyProfQueue/profilers/data*.
+The first *define_initialise* is there to add any variable declarations or code to the profiling bash script that would
+be needed in order to run the profiler. The second is any calls needed in order to terminate, or collect data post 
+running the profiler.
+
+If the profiler being added needs to be used in order to execute the user provided bash script, then the function 
+*define_run(profilefile: io.TextIOWrapper, bash_options: list, tmp_work_script: str)* should be defined in the 
+script for the specific profiler. This function should write the needed command to use the profilerto the profiling 
+file.
+___
 ___
 
 
 # To Do
 ___
 ___
-- Add in comments to describe all functions and improve readability of code
-- Reformat the location of the profiling functions to make adding more, easier
 - Update the package format to follow more modern conventions for installing requirements
   - e.g. add pyproject.toml 
 - Add Vtune profiling support
 - Add Linaro Forge profiling support
 ___
 ___
 # UKSRC related Links
```

### Comparing `PyProfQueue-0.2.0/PyProfQueue.egg-info/SOURCES.txt` & `PyProfQueue-0.2.1/PyProfQueue.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 setup.py
 PyProfQueue/__init__.py
-PyProfQueue/plot.py
 PyProfQueue/script.py
 PyProfQueue/submission.py
 PyProfQueue.egg-info/PKG-INFO
 PyProfQueue.egg-info/SOURCES.txt
 PyProfQueue.egg-info/dependency_links.txt
 PyProfQueue.egg-info/requires.txt
 PyProfQueue.egg-info/top_level.txt
```

### Comparing `PyProfQueue-0.2.0/ReadMe.md` & `PyProfQueue-0.2.1/ReadMe.md`

 * *Files 15% similar despite different names*

```diff
@@ -21,32 +21,24 @@
 ### Script Class
 The *Script* class is used in the following way, and the following options are available:
 ```
 script = PyProfQueue.Script(queue_system: str,
                             work_script: str,
                             read_queue_system: str =None,
                             queue_options: dict = None,
-                            likwid: bool = False,
-                            likwid_req: list = None,
-                            prometheus: bool = False,
-                            prometheus_ip: str = None, 
-                            prometheus_req: list = None
+                            profiling: dict = None
                             )   
 ```
-|           Option           | Description                                                                                                                                                                     |
-|:--------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-|        queue_system        | The intended target queue system (Supports Slurm and PBS Torque)                                                                                                                |
-|        work_script         | The bash script which contains the queue options and work to be done                                                                                                            |
-|read_queue_system (Optional)| The name of the queue system for which the script was written if it was written for a queue system                                                                              |
-|  queue_options (Optional)  | Any queue options to add or override when compared to the work_script                                                                                                           |
-|     likwid (Optional)      | Bool to determine if likwid should be used. Defaults to False.                                                                                                                  |
-|   likwid_req (Optional)    | Likwid requirements, details can be found in the section about **add_likwid**. Required if likwid Bool is True.                                                                 |
-|   prometheus (Optional)    | Bool to determine if prometheus should be used. Defaults to False.                                                                                                              |
-|  prometheus_ip (Optional)  | IP address of a pre-existing prometheus instance, not providing an address will result in launching a prometheus instance with the address 'http://localhost:9090'              |
-| prometheus_req (Optional)  | Prometheus requirements, details can be found in the section about **add_prometheus**. Required if prometheus Bool is True and no pre-existing prometheus instance is provided. |
+|           Option           | Description                                                                                                                        |
+|:--------------------------:|------------------------------------------------------------------------------------------------------------------------------------|
+|        queue_system        | The intended target queue system (Supports Slurm and PBS Torque)                                                                   |
+|        work_script         | The bash script which contains the queue options and work to be done                                                               |
+|read_queue_system (Optional)| The name of the queue system for which the script was written if it was written for a queue system                                 |
+|  queue_options (Optional)  | Any queue options to add or override when compared to the work_script                                                              |
+|    profiling (Optional)    | Dictionary with keys representing which profiler to use with values of dictionaries listing profiler options such as "requirements"|
 
 
 The options *queue_options* that PyProfQueue currently supports are:
 - 'user'
   - The user ID of the system with which to submit the job (requires admin rights usually)
 - 'nodes'
   - The number of nodes to be requested.
@@ -64,62 +56,15 @@
   - Name of the submitted job.
 - 'workdir'
   - The directory in which the work should be done.
 - 'output'
   - The file, including path, to write the STDOUT to.
 
 Any *Script* object, then comes with three additional methods intended to be used by users. These methods are:
-#### add_likwid
-```
-add_likwid(likwid_req: list)
-```
-- Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
-- This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
-- likwid_req is a list that should contain the necessary lines for the system in use to be able to use liquid. 
 
-For example, loading the likwid module:
-```
-likwid_req = ['module load likwid']
-```
-Example usage of *add_likwid* on a system that has the module environment, but where the likwid module requires the
-oneApi module to be loaded first:
-```
-script.add_likwid(likwid_req=['module load oneApi', 'module load likwid'])
-```
-#### add_prometheus
-```
-add_prometheus(prometheus_req: list, prometheus_ip: str = None)
-```
-- Adds necessary initiation to use measure computing resource usage
-- This can be used if a *Script* object was not initiated with prometheus options, or if they are to be changed
-- prometheus_req is a list that should contain the necessary lines for the system in use to be able to use
-prometheus. The example below shows how to define required environment variable **PROMETHEUS_SOFTWARE**. This variable
-needs to be the path to the prometheus software to be used. This only required if prometheus_ip is not being provided.
-- prometheus_ip is a string which is the ip-address of a pre-existing prometheus instance, if it exists.
-``` 
-prometheus_req = [
-    'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>'
-]
-```
-Example usage of *add_prometheus* where we provide the path to the **PROMETHEUS_SOFTWARE** directory:
-```
-script.add_prometheus(prometheus_req = ['export PROMETHEUS_SOFTWARE=/home/PrometheusSoftware'])
-```
-The **PROMETHEUS_SOFTWARE** directory should have the following structure at minimum, but may contain more files 
-depending on where it was stored and the version of node_exporter and prometheus being used.
-```md
-${PROMETHEUS_SOFTWARE}
-├── node_exporter
-│   └── node_exporter
-└── prometheus
-    ├── prometheus
-    └── prometheus.yml
-```
-Where *node_exporter/node_exporter* is the executable for node_exporter, *prometheus/prometheus* is the executable for 
-prometheus, and *prometheus/prometheus.yml* is the configuration file to be used for prometheus.
 #### change_options
 ```
 change_options(queue_options: dict)
 ```
 - Allows for options to be changed post initiation of a *Script* object, in case the options given in the 
 initialisation are no longer desired.
 
@@ -146,39 +91,102 @@
 |           script            | *Script* object to be submitted to queue                                                                                                                                                                           |
 | tmp_work_script (Optional)  | Desired name of temporary work script. Defaults to "tmp_workfile.sh".                                                                                                                                              |
 |tmp_profile_script (Optional)| Desired name of temporary profile script. Defaults to "tmp_profilefile.sh".                                                                                                                                        |
 |   bash_options (Optional)   | List of options that the user provided bash script may require. Defaults to [' '].                                                                                                                                 |
 |  leave_scripts (Optional)   | Boolean to determine if the temporary scripts should be left or removed after submission. Defaults to True                                                                                                         |
 |       test (Optional)       | Boolean to determine if the script should be submitted, or if the command that would be used should be printed to the terminal. Additionally, this leaves the temporary scripts in tackt so they can be inspected. |
 
-### plot_profiling function
-
-### plot_roof function
+### plot.load_df function
+This function reads the prometheus database created by using prometheus profiling with *PyProfQueue* and stores it 
+into a pandas.DataFrame. This then has the time converted into the format of "yyyy-mm-dd HH:MM:SS" for user readability.
+The times at which datapoints exist are then also given out as a numpy.array on top of returning the dataframe. 
+
+|    Option    | Description                             |
+|:------------:|-----------------------------------------|
+| feather_path | path to the scraped prometheus database |
+### plot.plot_profiling function
+This function plots the results of a prometheus profiling effort. It is compatible with additional features for 
+[Common Workflow Language](https://www.commonwl.org/) (CWL) workflows, if the output from a CWL call is saved to a file.
+
+|            Option            | Description                                                                                                                      |
+|:----------------------------:|----------------------------------------------------------------------------------------------------------------------------------|
+|              df              | pandas.DataFrame of the prometheus profiling data. Obtained from load_df                                                         |
+|         time_series          | numpy.array of the times at which data was collected. Obtained from load_df                                                      |
+|         name_prefix          | Desired path and name prefix for the plots                                                                                       |
+|network_three_mean (Optional) | Boolean on if the network y-limit should be restricted to three times the mean value                                             |
+|     mean_cpu (Optional)      | Boolean on if the mean_cpu usage should be plotted                                                                               |
+|      all_cpu (Optional)      | Boolean on if all cpu usages should be plotted                                                                                   |
+|      memory (Optional)       | Boolean on if the memory usage should be plotted                                                                                 |
+|      network (Optional)      | Boolean on if the network usage should be plotted                                                                                |
+|     cwl_file (Optional)      | Path to a text file containing the ouput of CWL, if it was used to run a workflow. This is used to shade when each step occured. |
+|       label (Optional)       | Boolean to label each CWL step on shaded graphs if cwl_file was provided                                                         |
+|       gant (Optional)        | Boolean on if a gant chart like plot should be created if CWL was used to run a workflow                                         |
+
+### plot.plot_roof function
+This function plots the results of a likwid profiling effort.
+
+|        Option         | Description                                                          |
+|:---------------------:|----------------------------------------------------------------------|
+|      name_prefix      | Desired path and name prefix for the plot                            |
+|        maxperf        | Float of the maximum performance listed in likwid output file        |
+|      maxband          | Float of the maximum memory bandwidth listed in likwid output file   |
+| code_name (Optional)  | String of what to call the code in the legend of the plot            |
+| code_mflop (Optional) | Float of the codes MFLOP/s listed in the likwid output               |
+| code_opint (Optional) | Float of the codes Operational Intensity listed in the likwid output |
 
 ___
 ##  In- and Outputs
 ___
 ### Inputs
 The inputs to the *Script* class and *submit* function have already been described above, what has not been described
 in detail in the input file that users provide. Users must provide the bash script that they wish to profile and submit
 to a queue system. If a bash script with no queue options is provided, then the *read_queue_system* option can be left
 off, or set to None. In this case, unless both *read_queue_system* and *queue_system* are set to None, *queue_options* 
 have to be provided. If queue options are available in the script then *read_queue_system* should be set to the name
 of the queue system that the original script was intended for.
+#### Likwid specific inputs
+In order to use likwid, the key 'likwid' needs to be used in the *profiling* option for the *Script* object. This key 
+then needs to have a value of "requirements" which contains a list of all commands that need to be executed prior to 
+being able to use likwid on the HPC system the script is being submitted to. If, for example, a simple module loading
+is required, it could look like this
+```python
+profiling = {"likwid": {"requirements":["module load likwid"]}}
+```
+#### Prometheus specific inputs
+In order to use prometheus, the key 'prometheus' needs to be used in the *profiling* option for the *Script* object. 
+This key then needs to have a value of "requirements" which has to contain the path to the prometheus instance to use, 
+or it has to contain "ip_address" which then has an IP address, stored as a string, of a pre-existing prometheus
+instance that can be scraped. Here is an example of both, where "<path/to/prometheus>" is used to represent the path
+to the prometheus instance the user would want to use.
+```python
+profiling = {"prometheus": {"requirements":["export PROMETHEUS_SOFTWARE=<path/to/prometheus>"]}}
+# OR
+profiling = {"prometheus": {"ip_address":["127.0.0.1:9090"]}}
+```
+
+#### Both likwid and prometheus
+Here is an example of how the dictionary could look, if both likwid and prometheus were to be used:
+```python
+profiling = {"likwid": {"requirements":["module load likwid"]}, 
+             "prometheus": {"requirements":["export PROMETHEUS_SOFTWARE=<path/to/prometheus>"]}
+             }
+```
 
 ### Outputs
 The output of the *Script* class, is an object that contains all the given options, file paths and other variables 
 needed in order to create the bash scripts that can be submitted to a queue system. The outputs from *submit* 
 depend on the given options. If the *test* and *leave_scripts* are set to **False**, then the output of *submit* is 
 the same as the output of the submission command for the respective queue system being used. If *test* or 
 *leave_scripts* are set to **True** then the output includes two bash scripts. The first contains the original work 
 to be performed, the other contains all the necessary variable declarations and command calls in order to perform 
 the profiling of the given bash script. It is the profiling script that is submitted to the queue. Additionally,
 if *test* is **True**, then the command line will output what command would be used in order to submit the job, but
 the command will not actually be called.
+
+For the plotting functions, the outputs are .png files of each requested plot.
 ___
 ## Example usage
 ___
 Let us look at a toy example to show how this script would be used. Let us assume we have an HPC system that uses slurm.
 This system requires loading the likwid module if we want to use it, and we have downloaded the prometheus codes to the
 directory **/home/Software** and ensured that we can execute both without sudo commands. Let us assume we have the 
 following bash script:
@@ -203,29 +211,28 @@
 submit the script to the queue. We have listed the queue options in the *Script* object initialisation even though it 
 would pull them from the bash script in order to show an example of how they would be listed.
 ```python 
 import PyProfQueue as ppq
 
 ProfileScript = ppq.Script(queue_system='slurm',
                            work_script='./tmp_workfile.sh',
-                           likwid=True,
-                           likwid_req=['module load likwid'],
-                           prometheus=True,
-                           prometheus_req=['export PROMETHEUS_SOFTWARE=/home/Software'],
                            queue_options={
                                'workdir': '/home/queue_work/%x.%j',
                                'account': 'example_project',
                                'cores': '16',
                                'nodes': '1',
                                'output': '/home/queue_work/%x.%j/output.out',
                                'partition': 'example_partition',
                                'name': 'TestSubmission',
                                'tasks': '1',
-                               'time': '00:05:00'
-                           })
+                               'time': '00:05:00'},
+                           profiling={"likwid": {'requirements': ['module load oneAPI_comp/2021.1.0',
+                                                                  'module load likwid/5.2.0']},
+                                      "prometheus": {'requirements': ['export PROMETHEUS_SOFTWARE=/home/Software']}
+                                      })
 
 ppq.submit(ProfileScript, 
            tmp_work_script = './test_workfile.sh',
            tmp_profile_script = './test_profilefile.sh',
            bash_options=['"Hello "', '"World!"'],
            test=True)
 ```
@@ -259,14 +266,15 @@
 ___
 ### Python Requirements
 For the sake of PyProfQueue, the required python version is at least 3.10, as this package utilises the match 
 functionality.
 - numpy
 - pytz
 - pyarrow
+- matplotlib
 - promql_http_api==0.3.3
 - pandas<=2.2.1
 ### Non Python Requirements
 In addition to the python requirements listed above, PyProfQueue also needs to have the following software on the system 
 to which the job will be submitted:
 - [node_exporter](https://prometheus.io/docs/guides/node-exporter/)
 - [prometheus](https://prometheus.io/)
@@ -288,63 +296,90 @@
 
 For the sake of likwid, it needs to be installed or loaded in, in such a way that a user could run the following 
 command without sudo rights:
 ```
 likwid-perfctr -g MEM_DP -f <executable>
 ```
 ___
-## Container Compatibility (If applicable)
+## Container Compatibility
 ___
 This package does not require a container and since it submits to a queue, we do not know how recommended it is to 
 use it from within a container.
 ___
 ## Hardware Requirements
 ___
 As of now, no minimum Hardware requirements are known other than those forced by python 3.10, prometheus, node_exporter
 and likwid.
 ___
 ## Directory Structure
 ___
 ```md
 PyProfQueue
 ├── PyProfQueue
-│   ├── data
-│   │   ├── read_prometheus.py
-│   │   ├── likwid_commands.txt
-│   │   └── prometheus_commands.txt
+│   ├── profilers
+│   │   ├── data
+│   │   │   ├── read_prometheus.py
+│   │   │   ├── _template_commands.txt
+│   │   │   ├── likwid_commands.txt
+│   │   │   └── prometheus_commands.txt
+│   │   ├── __init__.py
+│   │   ├── _template_profiler.py
+│   │   ├── likwid.py
+│   │   └── prometheus.py
 │   ├── __init__.py
 │   ├── plot.py
 │   ├── script.py
 │   └── submission.py
 ├── ReadMe.md
 └── setup.py
 ```
-The directory *PyProfQueue/data* contains a script called *read_prometheus.py* which is used to scrape the prometheus 
-database into a pandas dataframe. It also includes the two text files, *likwid_commands.txt* and 
-*prometheus_commands.txt*, which list the bash commands needed to initialise and end likwid and prometheus respectively.
+The directory *PyProfQueue/PyProfQueue* contains the *plot.py*. *script.py* and *submission.py* scripts which contain the 
+definition of the plotting functions, *Script* class and *submission()* function respectively.
+
+The directory *PyProfQueue/PyProfQueue/profilers* contains scripts of the individual profilers that PyProfQueue is 
+compatible with including a template version that can be used to add additional profiling software compatibility to 
+PyProfQueue. *PyProfQueue/PyProfQueue/profilers/data* contains a script called *read_prometheus.py* which is used to 
+scrape the prometheus database into a pandas dataframe. It also includes the text files that list the bash commands 
+needed to initialise run and end profiling software, as well as a template version for adding more profiling software 
+compatibility.
+
 
-The directory *PyProfQueue/PyProfQueue* contains the *script.py* and *submission.py* scripts which contain the 
-definition of the *Script* class and *submission()* function respectively.
 
 The base directory contains the ReadMe.md file, and the setup.py file so that the package can be installed.
 ___
 ## Adding new Queue systems
 ___
 A future goal for development on PyProfQueue is to add additional queue suport beyond slurm and torque. In order to add 
 new queue system compatibility refer to the block comments in the *Script* class in script.py. Each of the four section 
 that needs changes is marked with "Queue System specifics" followed by a {1}, {2}, {3} or {4}.
 ___
+## Adding new Profiling software
+___
+In order to add new profiling software compatibility, a new script would need to be added to the 
+*PyProfQueue/PyProfQueue/profilers* directory. This script would need to have the name of how the specific profiler
+should be called, as well as the following two functions:
+- define_initialise(profilefile: io.TextIOWrapper, profilerdict: dict = None)
+- define_end(profilefile: io.TextIOWrapper)
+
+Both of these functions can read from a .txt file, which can be stored in *PyProfQueue/PyProfQueue/profilers/data*.
+The first *define_initialise* is there to add any variable declarations or code to the profiling bash script that would
+be needed in order to run the profiler. The second is any calls needed in order to terminate, or collect data post 
+running the profiler.
+
+If the profiler being added needs to be used in order to execute the user provided bash script, then the function 
+*define_run(profilefile: io.TextIOWrapper, bash_options: list, tmp_work_script: str)* should be defined in the 
+script for the specific profiler. This function should write the needed command to use the profilerto the profiling 
+file.
+___
 ___
 
 
 # To Do
 ___
 ___
-- Add in comments to describe all functions and improve readability of code
-- Reformat the location of the profiling functions to make adding more, easier
 - Update the package format to follow more modern conventions for installing requirements
   - e.g. add pyproject.toml 
 - Add Vtune profiling support
 - Add Linaro Forge profiling support
 ___
 ___
 # UKSRC related Links
```

