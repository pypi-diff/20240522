# Comparing `tmp/DreamCreator-0.0.24.tar.gz` & `tmp/DreamCreator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DreamCreator-0.0.24.tar", last modified: Tue May 21 19:44:00 2024, max compression
+gzip compressed data, was "DreamCreator-0.0.3.tar", last modified: Wed Apr  3 23:41:02 2024, max compression
```

## Comparing `DreamCreator-0.0.24.tar` & `DreamCreator-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 19:44:00.060120 DreamCreator-0.0.24/
--rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 DreamCreator-0.0.24/LICENSE
--rw-rw-rw-   0        0        0     2494 2024-05-21 19:44:00.059120 DreamCreator-0.0.24/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 19:43:59.843767 DreamCreator-0.0.24/app/
-drwxrwxrwx   0        0        0        0 2024-05-21 19:43:59.874778 DreamCreator-0.0.24/app/DreamCreator.egg-info/
--rw-rw-rw-   0        0        0     2494 2024-05-21 19:43:58.000000 DreamCreator-0.0.24/app/DreamCreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2024-05-21 19:43:58.000000 DreamCreator-0.0.24/app/DreamCreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 19:43:58.000000 DreamCreator-0.0.24/app/DreamCreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2024-05-21 19:43:58.000000 DreamCreator-0.0.24/app/DreamCreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-21 19:43:58.000000 DreamCreator-0.0.24/app/DreamCreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 19:43:59.890766 DreamCreator-0.0.24/app/dreamcreator/
--rw-rw-rw-   0        0        0      114 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/__init__.py
--rw-rw-rw-   0        0        0    89472 2024-05-21 19:42:33.000000 DreamCreator-0.0.24/app/dreamcreator/sequencecreator.py
--rw-rw-rw-   0        0        0       68 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequencecreatorvariables.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:43:59.892767 DreamCreator-0.0.24/app/dreamcreator/sequences/
-drwxrwxrwx   0        0        0        0 2024-05-21 19:43:59.895766 DreamCreator-0.0.24/app/dreamcreator/sequences/BIO/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:24.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/BIO/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:43:59.937775 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:03.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/__init__.py
--rw-rw-rw-   0        0        0     2728 2024-05-01 18:00:31.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/current_sweep.py
--rw-rw-rw-   0        0        0     3285 2024-05-01 18:00:19.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_current_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3404 2024-04-29 21:16:26.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3056 2024-05-01 18:09:04.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_wavelength_current_sweep.py
--rw-rw-rw-   0        0        0     3575 2024-05-01 18:08:51.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
--rw-rw-rw-   0        0        0     2802 2024-05-01 18:06:34.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/voltage_sweep.py
--rw-rw-rw-   0        0        0     2807 2024-05-01 18:05:34.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/wavelength_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:44:00.006119 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:17.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/__init__.py
--rw-rw-rw-   0        0        0     2415 2024-05-01 22:40:23.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/current_sweep_ida.py
--rw-rw-rw-   0        0        0     3488 2024-05-01 18:01:26.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     3565 2024-05-01 23:03:32.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     2952 2024-05-01 18:03:17.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
--rw-rw-rw-   0        0        0     3038 2024-05-01 18:03:42.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2318 2024-05-01 22:39:41.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2490 2024-05-01 23:03:54.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0      112 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:44:00.041118 DreamCreator-0.0.24/app/dreamcreator/sequences/core/
--rw-rw-rw-   0        0        0      106 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/core/__init__.py
--rw-rw-rw-   0        0        0    10207 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/core/laser_sweep.py
--rw-rw-rw-   0        0        0    15635 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/core/results.py
--rw-rw-rw-   0        0        0     3086 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/core/sequence.py
--rw-rw-rw-   0        0        0     7492 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/core/smu_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:44:00.045119 DreamCreator-0.0.24/app/dreamcreator/sequences/template/
--rw-rw-rw-   0        0        0      971 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequences/template/__init__.py
--rw-rw-rw-   0        0        0     3071 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/sequencetracker.py
--rw-rw-rw-   0        0        0     4994 2024-04-04 20:31:52.000000 DreamCreator-0.0.24/app/dreamcreator/yamlcheck.py
--rw-rw-rw-   0        0        0       42 2024-05-21 19:44:00.061119 DreamCreator-0.0.24/setup.cfg
--rw-rw-rw-   0        0        0     1226 2024-05-21 19:43:18.000000 DreamCreator-0.0.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.274162 DreamCreator-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 DreamCreator-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1957 2024-04-03 23:41:02.273161 DreamCreator-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.168157 DreamCreator-0.0.3/app/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.184141 DreamCreator-0.0.3/app/DreamCreator.egg-info/
+-rw-rw-rw-   0        0        0     1957 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1511 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.196788 DreamCreator-0.0.3/app/dreamcreator/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.199784 DreamCreator-0.0.3/app/dreamcreator/File_edits/
+-rw-rw-rw-   0        0        0        0 2024-03-28 21:58:12.000000 DreamCreator-0.0.3/app/dreamcreator/File_edits/__init__.py
+-rw-rw-rw-   0        0        0       31 2024-01-24 23:45:27.000000 DreamCreator-0.0.3/app/dreamcreator/__init__.py
+-rw-rw-rw-   0        0        0    62177 2024-03-28 22:14:35.000000 DreamCreator-0.0.3/app/dreamcreator/sequencecreator.py
+-rw-rw-rw-   0        0        0       68 2024-01-23 01:45:18.000000 DreamCreator-0.0.3/app/dreamcreator/sequencecreatorvariables.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.235163 DreamCreator-0.0.3/app/dreamcreator/sequences/
+-rw-rw-rw-   0        0        0      112 2024-01-23 01:45:18.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.246166 DreamCreator-0.0.3/app/dreamcreator/sequences/core/
+-rw-rw-rw-   0        0        0      106 2024-01-23 01:45:18.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/__init__.py
+-rw-rw-rw-   0        0        0    10207 2024-03-28 22:17:23.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/laser_sweep.py
+-rw-rw-rw-   0        0        0    15635 2024-01-23 01:45:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/results.py
+-rw-rw-rw-   0        0        0     3086 2024-03-28 22:17:29.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/sequence.py
+-rw-rw-rw-   0        0        0     7492 2024-03-28 22:17:32.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/smu_sweep.py
+-rw-rw-rw-   0        0        0     2409 2024-03-28 22:15:55.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep.py
+-rw-rw-rw-   0        0        0     2044 2024-03-28 22:15:49.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep_ida.py
+-rw-rw-rw-   0        0        0     2476 2024-03-28 22:16:02.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     2884 2024-03-28 22:15:58.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     2793 2024-03-28 22:16:08.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     2974 2024-03-28 22:16:05.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     2549 2024-03-28 22:16:14.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep.py
+-rw-rw-rw-   0        0        0     2508 2024-03-28 22:16:11.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep_ida.py
+-rw-rw-rw-   0        0        0     2918 2024-03-28 22:16:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_voltage_sweep.py
+-rw-rw-rw-   0        0        0     2603 2024-03-28 22:16:17.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_voltage_sweep_ida.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.249163 DreamCreator-0.0.3/app/dreamcreator/sequences/template/
+-rw-rw-rw-   0        0        0      971 2024-01-23 01:45:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/template/__init__.py
+-rw-rw-rw-   0        0        0     2273 2024-03-28 22:16:25.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/voltage_sweep.py
+-rw-rw-rw-   0        0        0     1952 2024-03-28 22:16:22.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2260 2024-03-28 22:16:36.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep.py
+-rw-rw-rw-   0        0        0     2033 2024-03-28 22:16:28.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     3071 2024-01-23 01:45:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequencetracker.py
+-rw-rw-rw-   0        0        0     4334 2024-01-23 01:45:51.000000 DreamCreator-0.0.3/app/dreamcreator/yamlcheck.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 23:41:02.274162 DreamCreator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2024-04-03 23:40:55.000000 DreamCreator-0.0.3/setup.py
```

### Comparing `DreamCreator-0.0.24/LICENSE` & `DreamCreator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.24/PKG-INFO` & `DreamCreator-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 Metadata-Version: 2.1
 Name: DreamCreator
-Version: 0.0.24
+Version: 0.0.3
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/dreamphotonics/DreamCreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Title
 
-This package is for use in Dream Photonics or the UBC Photonics edx course, and contains utilities for creating
-yaml files which act as guides for tests on the probe stations throughout UBC.
+Simple overview of use/purpose.
 
 ## Description
 
-This software contains a User Interface that easily allows users to create custom YAML files to guide tests on probe stations throughout UBC. It is built using PyQt and leverages the dreamcreator and sequencecreator modules for functionality. To add a new stage setup simply add an additional folder in the sequences directory and populate with formatted sequence files, then reload the UI.
+An in-depth paragraph about your project and overview of use.
 
 ## Getting Started
 
 ### Dependencies
 
 * Describe any prerequisites, libraries, OS version, etc., needed before installing program.
 * ex. Windows 10
-python: 3.11
-Windows: 10 or greater
-
 
 ### Installing
 
 * How/where to download your program
 * Any modifications needed to be made to files/folders
 
 ### Executing program
 
 * How to run the program
+* Step-by-step bullets
 ```
-import dreamcreator
-from dreamcreator import sequencecreator as sc
-sc.launch()
+code blocks for commands
 ```
 
 ## Help
 
 Any advise for common problems or issues.
 ```
 command to run if program contains helper info
 ```
 
 ## Authors
 
 Contributors names and contact info
 
-Jon Barnes [@JonBarnes](https://twitter.com/JonBarnes)
+ex. Dominique Pizzie  
+ex. [@DomPizzie](https://twitter.com/dompizzie)
 
 ## Version History
 
 * 0.2
     * Various bug fixes and optimizations
     * See [commit change]() or See [release history]()
 * 0.1
     * Initial Release
 
 ## License
 
-This project is licensed under the MIT License - see the LICENSE.md file for details
+This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
 
 ## Acknowledgments
 
 Inspiration, code snippets, etc.
 * [awesome-readme](https://github.com/matiassingers/awesome-readme)
 * [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
 * [dbader](https://github.com/dbader/readme-template)
```

### Comparing `DreamCreator-0.0.24/app/DreamCreator.egg-info/PKG-INFO` & `DreamCreator-0.0.3/app/DreamCreator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 Metadata-Version: 2.1
 Name: DreamCreator
-Version: 0.0.24
+Version: 0.0.3
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/dreamphotonics/DreamCreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Title
 
-This package is for use in Dream Photonics or the UBC Photonics edx course, and contains utilities for creating
-yaml files which act as guides for tests on the probe stations throughout UBC.
+Simple overview of use/purpose.
 
 ## Description
 
-This software contains a User Interface that easily allows users to create custom YAML files to guide tests on probe stations throughout UBC. It is built using PyQt and leverages the dreamcreator and sequencecreator modules for functionality. To add a new stage setup simply add an additional folder in the sequences directory and populate with formatted sequence files, then reload the UI.
+An in-depth paragraph about your project and overview of use.
 
 ## Getting Started
 
 ### Dependencies
 
 * Describe any prerequisites, libraries, OS version, etc., needed before installing program.
 * ex. Windows 10
-python: 3.11
-Windows: 10 or greater
-
 
 ### Installing
 
 * How/where to download your program
 * Any modifications needed to be made to files/folders
 
 ### Executing program
 
 * How to run the program
+* Step-by-step bullets
 ```
-import dreamcreator
-from dreamcreator import sequencecreator as sc
-sc.launch()
+code blocks for commands
 ```
 
 ## Help
 
 Any advise for common problems or issues.
 ```
 command to run if program contains helper info
 ```
 
 ## Authors
 
 Contributors names and contact info
 
-Jon Barnes [@JonBarnes](https://twitter.com/JonBarnes)
+ex. Dominique Pizzie  
+ex. [@DomPizzie](https://twitter.com/dompizzie)
 
 ## Version History
 
 * 0.2
     * Various bug fixes and optimizations
     * See [commit change]() or See [release history]()
 * 0.1
     * Initial Release
 
 ## License
 
-This project is licensed under the MIT License - see the LICENSE.md file for details
+This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
 
 ## Acknowledgments
 
 Inspiration, code snippets, etc.
 * [awesome-readme](https://github.com/matiassingers/awesome-readme)
 * [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
 * [dbader](https://github.com/dbader/readme-template)
```

### Comparing `DreamCreator-0.0.24/app/DreamCreator.egg-info/SOURCES.txt` & `DreamCreator-0.0.3/app/DreamCreator.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,31 +6,29 @@
 app/DreamCreator.egg-info/requires.txt
 app/DreamCreator.egg-info/top_level.txt
 app/dreamcreator/__init__.py
 app/dreamcreator/sequencecreator.py
 app/dreamcreator/sequencecreatorvariables.py
 app/dreamcreator/sequencetracker.py
 app/dreamcreator/yamlcheck.py
+app/dreamcreator/File_edits/__init__.py
 app/dreamcreator/sequences/__init__.py
-app/dreamcreator/sequences/BIO/__init__.py
-app/dreamcreator/sequences/DREAM/__init__.py
-app/dreamcreator/sequences/DREAM/current_sweep.py
-app/dreamcreator/sequences/DREAM/set_current_wavelength_sweep.py
-app/dreamcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
-app/dreamcreator/sequences/DREAM/set_wavelength_current_sweep.py
-app/dreamcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
-app/dreamcreator/sequences/DREAM/voltage_sweep.py
-app/dreamcreator/sequences/DREAM/wavelength_sweep.py
-app/dreamcreator/sequences/IDA/__init__.py
-app/dreamcreator/sequences/IDA/current_sweep_ida.py
-app/dreamcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
-app/dreamcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
-app/dreamcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
-app/dreamcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
-app/dreamcreator/sequences/IDA/voltage_sweep_ida.py
-app/dreamcreator/sequences/IDA/wavelength_sweep_ida.py
+app/dreamcreator/sequences/current_sweep.py
+app/dreamcreator/sequences/current_sweep_ida.py
+app/dreamcreator/sequences/set_current_wavelength_sweep.py
+app/dreamcreator/sequences/set_current_wavelength_sweep_ida.py
+app/dreamcreator/sequences/set_voltage_wavelength_sweep.py
+app/dreamcreator/sequences/set_voltage_wavelength_sweep_ida.py
+app/dreamcreator/sequences/set_wavelength_current_sweep.py
+app/dreamcreator/sequences/set_wavelength_current_sweep_ida.py
+app/dreamcreator/sequences/set_wavelength_voltage_sweep.py
+app/dreamcreator/sequences/set_wavelength_voltage_sweep_ida.py
+app/dreamcreator/sequences/voltage_sweep.py
+app/dreamcreator/sequences/voltage_sweep_ida.py
+app/dreamcreator/sequences/wavelength_sweep.py
+app/dreamcreator/sequences/wavelength_sweep_ida.py
 app/dreamcreator/sequences/core/__init__.py
 app/dreamcreator/sequences/core/laser_sweep.py
 app/dreamcreator/sequences/core/results.py
 app/dreamcreator/sequences/core/sequence.py
 app/dreamcreator/sequences/core/smu_sweep.py
 app/dreamcreator/sequences/template/__init__.py
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequencecreator.py` & `DreamCreator-0.0.3/app/dreamcreator/sequencecreator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,78 @@
-# %%
-from pathlib import Path
+#%%
 from PyQt5.QtWidgets import (
     QApplication,
     QTextEdit,
     QWidget,
     QVBoxLayout,
     QHBoxLayout,
     QPushButton,
     QFileDialog,
     QLabel,
     QLineEdit,
     QListWidget,
     QListWidgetItem,
     QMessageBox,
-    QCheckBox,
-    QComboBox,
+    QCheckBox
 )
-from PyQt5.QtCore import Qt, pyqtSignal, QObject
-from PyQt5.QtWidgets import QLabel, QLineEdit, QVBoxLayout, QWidget, QFormLayout
+from PyQt5.QtCore import Qt
+from PyQt5.QtGui import QPalette, QColor
 import os
 from os.path import dirname, abspath
 import sys
 import ast
 import yaml
 import importlib
+# from dreamstest.chip import ElectroOpticDevice
+from PyQt5.QtWidgets import QLabel, QLineEdit, QVBoxLayout, QWidget, QFormLayout
+import os
 import importlib.util
 import inspect
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
-import logging
 from dreamcreator.yamlcheck import yaml_check
+import sys
+import logging
+from PyQt5.QtWidgets import QApplication, QWidget, QVBoxLayout, QTextEdit
+from PyQt5.QtCore import pyqtSignal, QObject
+
 
 
 def launch():
     app = QApplication([])
     ex = GUI()
     ex.show()
     app.exec_()
 
 
 class GUI(QWidget):
     def __init__(self):
         super().__init__()
-        self.setWindowTitle("Dream Creator")
-        self.custom_sequences_store = dict()
-        self.branch = 'IDA'
 
+        
         self.yamldict = dict()
         self.yamldict = {"Devices": {}, "Sequences": {}}
-        self.runtime_journal = dict()
 
         # Set up the layout
         self.layout = QVBoxLayout()
         self.hlayout = QHBoxLayout()
         self.setLayout(self.layout)
 
         # Set up the file selection area
-        #self.setup_yaml_selection()
+        self.setup_yaml_selection()
         self.setup_file_selection()
 
         # Set up the sequence selection area
         self.setup_sequence_selection()
 
         # Set up the group and devices area
         self.setup_devices()
 
         self.layout.addLayout(self.hlayout)
-        #self.setup_save_folder()
+        self.setup_save_folder()
 
         self.setup_outputlog()
         self.removed_items = self.remove_non_ida_entries(self.sequences_checklist)
 
     def setup_outputlog(self):
         # Set up the output log
         self.outputtitle = QLabel("Output Log")
@@ -78,45 +80,44 @@
 
         # Log Viewer
 
         self.logTextBox = QTextEditLogger(self)
         self.layout.addWidget(self.logTextBox.widget)
 
         # Set up logging
-        logging.basicConfig(
-            format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
-        )
+        logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s',
+                            level=logging.INFO)
         log = logging.getLogger()
         log.addHandler(self.logTextBox)
 
         # Test logging
-        # logging.info("This is an informational message.")
+        #logging.info("This is an informational message.")
 
         # Redirect standard output to logging
-        std_out_logger = logging.getLogger("STDOUT")
+        std_out_logger = logging.getLogger('STDOUT')
         sl = StreamToLogger(std_out_logger, logging.INFO)
         sys.stdout = sl
 
-        # self.outputtitle = QLabel("Output Log")
+        #self.outputtitle = QLabel("Output Log")
         # self.layout.addWidget(self.outputtitle)
 
         # self.textEdit = QTextEdit()
         # self.textEdit.setReadOnly(True)
 
         # # Redirect stdout and stderr
         # sys.stdout = StreamRedirector(self.textEdit)
         # sys.stderr = StreamRedirector(self.textEdit)
 
         # self.layout.addWidget(self.textEdit)
 
     def setup_file_selection(self):
-        self.file_title = QLabel("Upload coordinates file or Yaml file")
+        self.file_title = QLabel("Upload coordinates file")
         self.file_label = QLineEdit("No file selected")
         self.file_button = QPushButton("Choose File")
-        self.file_button.clicked.connect(self.choose_file)
+        self.file_button.clicked.connect(self.choose_coord_file)
 
         file_layoutv = QVBoxLayout()
         file_layout = QHBoxLayout()
         file_layoutv.addWidget(self.file_title)
         file_layout.addWidget(self.file_label)
         file_layout.addWidget(self.file_button)
         file_layoutv.addLayout(file_layout)
@@ -132,75 +133,46 @@
         file_layout = QHBoxLayout()
         file_layoutv.addWidget(self.yfile_title)
         file_layout.addWidget(self.yfile_label)
         file_layout.addWidget(self.yfile_button)
         file_layoutv.addLayout(file_layout)
         self.layout.addLayout(file_layoutv)
 
-    def get_sequences_path(self, branch=None):
-    # Determine if running from executable or regular script
-        if getattr(sys, 'frozen', False):  
-            # Running from executable
-            data_dir = Path(sys._MEIPASS)  # Temporary extraction directory
-        else:
-            # Running as a regular script
-            data_dir = Path(__file__).parent.resolve() 
-
-        if branch:
-            sequences_path = data_dir / "sequences" / branch
-        else:
-            sequences_path = data_dir / "sequences"
-        return str(sequences_path.resolve())
-
-    def place_sequence_options(self):
-        #if self.branch:
-        #p = dirname(abspath(__file__))
-
-        p = self.get_sequences_path(self.branch)
+    def setup_sequence_selection(self):
+        p = dirname(abspath(__file__))
 
-        #print(p)
-
-        sequences_dict = DirectoryDict(p)
+        sequences_dict = DirectoryDict(os.path.join(p, 'sequences'))
 
         self.sequences_checklist = self.create_checklist(sequences_dict.dir_dict)
         self.sequence_versions_checklist = self.create_checklist(
             sequences_dict.dir_dict
         )
         custom_sequences_dict = self.yamldict["Sequences"]
         self.customsequences_checklist = self.create_checklist(
             custom_sequences_dict, customflag=True
         )
-
-    def setup_sequence_selection(self, branch='IDA'):
-
-        self.place_sequence_options()
-        
         sequence_hlayout = QHBoxLayout()
-        self.sequence_layout = QVBoxLayout()
+        sequence_layout = QVBoxLayout()
         edxchoicelayout = QHBoxLayout()
 
-
-        self.create_checkboxes(edxchoicelayout)
-
-        # self.checkBox1 = QCheckBox("IDA")
-        # self.checkBox1.setChecked(True)
-        # self.IDAcheck = True
-        # self.checkBox2 = QCheckBox("DREAM")
-        # self.checkbox3 = QCheckBox("BIO")
-
-        #edxchoicelayout.addWidget(self.checkBox1)
-        #edxchoicelayout.addWidget(self.checkBox2)
-        #self.checkBox1.stateChanged.connect(self.update_checkboxes)
-        #self.checkBox2.stateChanged.connect(self.update_checkboxes)
-        self.sequence_layout.addLayout(edxchoicelayout)
-
-        self.sequence_layout.addWidget(QLabel("Sequences"))
-        self.sequence_layout.addWidget(self.sequences_checklist)
-        self.sequence_layout.addWidget(QLabel("Custom Sequences"))
-        self.sequence_layout.addWidget(self.customsequences_checklist)
+        self.checkBox1 = QCheckBox("edx course")
+        self.checkBox1.setChecked(True)
+        self.edxcheck = True
+        self.checkBox2 = QCheckBox("Internal Use")
+
+        edxchoicelayout.addWidget(self.checkBox1)
+        edxchoicelayout.addWidget(self.checkBox2)
+        self.checkBox1.stateChanged.connect(self.update_checkboxes)
+        self.checkBox2.stateChanged.connect(self.update_checkboxes)
+        sequence_layout.addLayout(edxchoicelayout)
+
+        sequence_layout.addWidget(QLabel("Sequences"))
+        sequence_layout.addWidget(self.sequences_checklist)
+        sequence_layout.addWidget(QLabel("Custom Sequences"))
+        sequence_layout.addWidget(self.customsequences_checklist)
 
         self.parameters_area = QWidget()
 
         sequence_variables_layout = QVBoxLayout()
         sequence_variables_layout.addWidget(QLabel("Sequence Variables"))
         sequence_variables_layout.addWidget(self.parameters_area)
 
@@ -208,91 +180,38 @@
         self.sequence_namer = QLineEdit()
         self.SetButton = QPushButton("Set Sequence")
         self.SetButton.clicked.connect(self.set_sequence)
         buttonhlayout.addWidget(self.sequence_namer)
         buttonhlayout.addWidget(self.SetButton)
 
         sequence_variables_layout.addLayout(buttonhlayout)
-        sequence_hlayout.addLayout(self.sequence_layout)
+        sequence_hlayout.addLayout(sequence_layout)
         sequence_hlayout.addLayout(sequence_variables_layout)
 
         self.hlayout.addLayout(sequence_hlayout)
 
-    def replace_widget(self, layout, widget_to_replace, custom_widget_to_replace, custom=False):
-        #self.custom_sequences_store[self.branch] = widget_to_replace
-        index = layout.indexOf(widget_to_replace)
-        custom_index = layout.indexOf(custom_widget_to_replace)
-        widget_to_replace.hide()       
-        custom_widget_to_replace.hide()  
-        # if not custom: 
-        widget_to_replace.deleteLater()
-        custom_widget_to_replace.deleteLater()
-        self.place_sequence_options() 
-        # if custom:
-        #     layout.insertWidget(self.custom_sequences_store[self.old_branch], self.customsequences_checklist)
-        # else:
-        
-        layout.insertWidget(index, self.sequences_checklist)
-        layout.insertWidget(custom_index, self.customsequences_checklist)
-        
-
-        #self.replace_custom_widget(layout)
-
-    def create_checkboxes(self, layout):
-        """Finds the names of folders in the current working directory.
-
-        Returns:
-            A list of folder names.
-        """
-
-        folder_names = []
-
-        script_dir = Path(__file__).parent.resolve()  # Ensure absolute path
-        # Define the relative path *within your project*
-        rel_path = Path("sequences")
-        # Combine the script directory with the relative path to get the full path
-        mypath = script_dir / rel_path
-        # Resolve the full path on the system
-        dir_path = str(mypath.resolve())
-
-        dir_path = self.get_sequences_path()
-        self.checkboxes = []
-
-        #print(dir_path)
-
-        for entry in os.listdir(dir_path):  # Iterate over entries in the directory
-            
-            if entry != 'core' and entry != '__pycache__' and entry != 'template' and entry != '__init__.py':
-                self.checkBox = QCheckBox(entry)
-                self.checkBox.setObjectName(entry)
-                self.checkboxes.append(self.checkBox)
-                self.checkBox.clicked.connect(self.update_checkboxes)
-                if entry == 'IDA':
-                    self.checkBox.setChecked(True)
-                layout.addWidget(self.checkBox)
-
     def remove_non_ida_entries(self, checklist: QListWidget):
         """Removes checklist entries not ending with '_ida' and returns the removed items.
 
         Args:
             checklist: The PyQt5 QListWidget object to modify.
 
         Returns:
             A list of the text labels of the removed items.
         """
 
         removed_items = []
         for i in reversed(range(checklist.count())):
             item = checklist.item(i)
-            if not item.text().endswith("_ida"):
+            if not item.text().endswith('_ida'):
                 removed_items.append(item.text())  # Store before removing
                 checklist.takeItem(i)
 
         return removed_items
-
+    
     def add_removed_entries(self, checklist: QListWidget, removed_items):
         """Adds previously removed entries back to the checklist with checkboxes.
 
         Args:
             checklist: The PyQt5 QListWidget object to modify.
             removed_items: A list of the text labels of the removed items.
         """
@@ -312,76 +231,34 @@
 
         Returns:
             A list of the text labels of the removed items.
         """
         removed_items = []
         for i in reversed(range(checklist.count())):
             item = checklist.item(i)
-            if "_ida" in item.text():
+            if '_ida' in item.text():
                 removed_items.append(item.text())  # Store before removing
-                checklist.takeItem(i)
+                checklist.takeItem(i) 
 
         return removed_items
+    
 
     def update_checkboxes(self, item):
         sender = self.sender()
-        name = sender.objectName()
-        checkbox = self.findChild(QCheckBox, name)
-
-        check = self.warning_popup()
-
-        if check:
-            if checkbox:
-                for box in self.checkboxes:
-                    if box.objectName() != checkbox.objectName():
-                        if box.isChecked():
-                            box.setChecked(False)
-
-            #self.custom_sequences_store[self.branch] = self.customsequences_checklist
-            self.old_branch = self.branch
-            self.branch = name
-            #if checkbox:
-            # self.replace_widget(self.sequence_layout, self.customsequences_checklist, custom=True)
-            self.yamldict['Sequences'] = {}
-            #self.place_sequence_options()
-
-            if checkbox:
-                self.replace_widget(self.sequence_layout, self.sequences_checklist, self.customsequences_checklist)
-        else:
-            checkbox.setChecked(False)
-
-        # checkbox.setChecked(True)
-
-        # if sender.isChecked():
-        #     if sender == self.checkBox1:
-        #         self.IDAcheck = True
-        #         self.checkBox2.setChecked(False)
-        #         self.add_removed_entries(self.sequences_checklist, self.removed_items)
-        #         self.removed_items = self.remove_non_ida_entries(
-        #             self.sequences_checklist
-        #         )
-        #     elif sender == self.checkBox2:
-        #         self.IDAcheck = False
-        #         self.checkBox1.setChecked(False)
-        #         self.add_removed_entries(self.sequences_checklist, self.removed_items)
-        #         self.removed_items = self.remove_ida_entries(self.sequences_checklist)
-
-    def warning_popup(self):
-        popup = QMessageBox()
-        popup.setWindowTitle("Warning")
-        popup.setText('Warning: if you change stage all custom sequences will be erased')
-        popup.addButton('Continue', QMessageBox.AcceptRole)
-        popup.addButton('Cancel', QMessageBox.RejectRole)
-
-        result = popup.exec()
-
-        if result == QMessageBox.AcceptRole:
-            return True
-        else:
-            return False
+        if sender.isChecked():
+            if sender == self.checkBox1:
+                self.edxcheck = True
+                self.checkBox2.setChecked(False)
+                self.add_removed_entries(self.sequences_checklist, self.removed_items)
+                self.removed_items = self.remove_non_ida_entries(self.sequences_checklist)
+            elif sender == self.checkBox2:
+                self.edxcheck = False
+                self.checkBox1.setChecked(False)
+                self.add_removed_entries(self.sequences_checklist, self.removed_items)
+                self.removed_items = self.remove_ida_entries(self.sequences_checklist)
 
     def button1_clicked(self, item):
         selected_devices = []
         selected_sequence = []
 
         # check which devices is selected
         for i in range(self.listbox2.count()):
@@ -394,59 +271,44 @@
             if self.customsequences_checklist.item(i).checkState() == Qt.Checked:
                 selected_sequence.append(self.customsequences_checklist.item(i))
 
         # check which sequence is selected
 
         # selected_sequence = self.customsequences_checklist.selectedItems()
 
-
-        if selected_sequence != [] and selected_devices != []:
+        if selected_sequence != [] or selected_devices != []:
             for device in selected_devices:
                 self.yamldict["Devices"][device.text()]["sequences"].append(
-                    selected_sequence[0].text().split(' ')[0]
+                    selected_sequence[0].text()
                 )
-                seq = selected_sequence[0].text().split(' ')[0]
-                self.runtime_journal[seq][1] = self.runtime_journal[seq][1] + 1
                 print(
                     "Linked sequence: "
                     + selected_sequence[0].text()
-                    + " and device: "
+                    + "and device: "
                     + device.text()
                 )
 
-            sequence_item = QListWidgetItem(selected_sequence[0].text().split(' ')[0])
-            sequence_item.setFlags(sequence_item.flags() | Qt.ItemIsUserCheckable)
-            sequence_item.setCheckState(Qt.Unchecked) 
-            self.listbox4.addItem(sequence_item)
-        else:
-            print('Please make sure a sequence and device(s) are selected before linking.')
-
     def button2_clicked(self, item):
         options = QFileDialog.Options()
         filename, _ = QFileDialog.getSaveFileName(
             None,
             "Save as YAML",
             "",
             "YAML Files (*.yaml);;All Files (*)",
             options=options,
         )
-        settime = 10000
-        runtime = self.total_runtime_check(self.yamldict)
-        if runtime >= settime:
-            print(f"Total runtime {runtime} exceeds set threshold of {settime}, aborting save.")
+
+        if filename:
+            if not filename.endswith(".yaml"):
+                filename += ".yaml"
+            with open(filename, "w") as file:
+                yaml.dump(self.yamldict, file)
+            print("Saved to " + filename)
         else:
-            print(f"Total runtime {runtime} is within set threshold of {settime}, proceeding with save.")
-            if filename:
-                if not filename.endswith(".yaml"):
-                    filename += ".yaml"
-                with open(filename, "w") as file:
-                    yaml.dump(self.yamldict, file)
-                print("Saved to " + filename)
-            else:
-                print("Please choose save location to export YAML file.")
+            print('Please choose save location to export YAML file.')
 
     def object_to_dict(self, obj):
         """
         Convert an object's attributes to a dictionary.
 
         Args:
         - obj: The object to be converted
@@ -467,21 +329,18 @@
         Args:
             checklist (QListWidget): The checklist to refresh.
             data_dict (dict): Dictionary containing data for the checklist.
         """
         checklist.clear()  # Clear existing items
 
         for key in data_dict:
-            if 'Runtime' in data_dict[key]:
-                item = QListWidgetItem(key + ' [' + str(data_dict[key]['Runtime']) + ' secs' ']')
-                self.runtime_journal[key] = [data_dict[key]['Runtime'], 0]
-            else:
-                self.sequence_runtime_check(self.extract_text_in_brackets(key), data_dict[key], key)
-                item = QListWidgetItem(key + ' [' + str(data_dict[key]['Runtime']) + ' secs' ']')
-            item.setFlags(item.flags() | Qt.ItemIsUserCheckable)  # Allow user to check/uncheck the item
+            item = QListWidgetItem(key)
+            item.setFlags(
+                item.flags() | Qt.ItemIsUserCheckable
+            )  # Allow user to check/uncheck the item
             item.setCheckState(Qt.Unchecked)  # Initially set the item to unchecked
             checklist.addItem(item)
 
     def setup_buttons(self):
         button1 = QPushButton("Link Sequence")
         button2 = QPushButton("Button 2")
         button3 = QPushButton("Button 3")
@@ -496,71 +355,49 @@
         self.layout.addLayout(buttons_layout)
 
     def setup_devices(self):
         layoutv = QVBoxLayout()
 
         button1 = QPushButton("Link Sequence")
         button2 = QPushButton("Export Yaml")
-        #button3 = QPushButton("Adjust coord file")
+        button3 = QPushButton("Adjust coord file")
 
         buttons_layout = QHBoxLayout()
         buttons_layout.addWidget(button1)
         buttons_layout.addWidget(button2)
-        #buttons_layout.addWidget(button3)
+        buttons_layout.addWidget(button3)
 
         button1.clicked.connect(self.button1_clicked)
         button2.clicked.connect(self.button2_clicked)
-        #button3.clicked.connect(self.fix_coord_file)
+        button3.clicked.connect(self.fix_coord_file)
 
         layoutv.addLayout(buttons_layout)
 
         layouth = QHBoxLayout()
         self.listbox1 = QListWidget()
         self.listbox1_2 = QListWidget()
         self.listbox1_3 = QListWidget()
         self.listbox2 = QListWidget()
         self.listbox2.setSelectionMode(QListWidget.ExtendedSelection)
 
         devices_group_layout = QVBoxLayout()
-        self.device_search = QLineEdit()
-        self.device_search.setPlaceholderText("Search for devices here...")
-        self.device_search.textChanged.connect(self.search_devices)
+        device_search = QLineEdit()
+        device_search.textChanged.connect(self.search_devices)
 
-        devices_group_layout.addWidget(self.device_search)
+        devices_group_layout.addWidget(device_search)
         devices_group_layout.addWidget(QLabel("Devices"))
         devices_group_layout.addWidget(self.listbox2)
 
-        button_h_layout = QHBoxLayout()
-
         select_all_btn = QPushButton("Select All")
         select_all_btn.clicked.connect(self.select_all)
-
-        button_h_layout.addWidget(select_all_btn)
-
-        unselect_all_btn = QPushButton("Unselect All")
-        unselect_all_btn.clicked.connect(self.unselect_all)
-
-        button_h_layout.addWidget(unselect_all_btn)
-
-        selectkw_btn = QPushButton("Select Keyword")
-        selectkw_btn.clicked.connect(self.select_keyword)
-
-        button_h_layout.addWidget(selectkw_btn)
-
-        select_highlighted_btn = QPushButton("Select Highlighted")
-        select_highlighted_btn.clicked.connect(self.select_highlighted)
-
-        button_h_layout.addWidget(select_highlighted_btn)
-
-        devices_group_layout.addLayout(button_h_layout)
-
-
+        devices_group_layout.addWidget(select_all_btn)
 
         choice_menu = QHBoxLayout()
 
+
         grouplayout = QVBoxLayout()
         grouplayout.addWidget(QLabel("Group"))
         grouplayout.addWidget(self.listbox1)
         self.listbox1.setFixedWidth(75)
         choice_menu.addLayout(grouplayout)
 
         pollayout = QVBoxLayout()
@@ -584,117 +421,24 @@
         self.listbox4 = QListWidget()
 
         device_data_sequences_layout = QVBoxLayout()
         device_data_sequences_layout.addWidget(QLabel("Device Data"))
         device_data_sequences_layout.addWidget(self.listbox3)
         device_data_sequences_layout.addWidget(QLabel("Associated Sequences"))
         device_data_sequences_layout.addWidget(self.listbox4)
-        self.listbox4.itemChanged.connect(self.on_itembox4_checked)
-
-        remove_sequence_btn = QPushButton("Remove Sequence")
-        remove_sequence_btn.clicked.connect(self.remove_sequence)
-        device_data_sequences_layout.addWidget(remove_sequence_btn)
 
         layoutv.addLayout(device_data_sequences_layout)
         layouth.addLayout(layoutv)
 
         self.hlayout.addLayout(layouth)
 
-    def select_items(self, sequence_name):
-        for i in range(self.listbox2.count()):
-            item = self.listbox2.item(i)
-            try:
-                if sequence_name in self.devicedict[item.text()]['sequences']:
-                    item.setSelected(True)
-            except:
-                for x in self.deviceobjects:
-                    a = item.text()
-                    b = x.device_id
-                    if item.text() == x.device_id:
-                        deviceobject = x
-                if sequence_name in deviceobject.sequences:
-                    item.setSelected(True)
-
-    def unselect_items(self):
-        for i in range(self.listbox2.count()):
-            item = self.listbox2.item(i)
-            item.setSelected(False)
-
-    def on_itembox4_checked(self):
-        checked_items = self.find_checked_items(self.listbox4)
-        if len(checked_items) == 1:
-
-            self.select_items(checked_items[0].text())
-
-            for i in range(self.customsequences_checklist.count()):
-                if self.customsequences_checklist.item(i).text() != checked_items[0].text():
-                    self.customsequences_checklist.item(i).setCheckState(Qt.Unchecked)
-                else:
-                    self.customsequences_checklist.item(i).setCheckState(Qt.Checked)
-
-
-            
-            self.custom_reset_parameters(checked_items[0].text().split(' ')[0])
-            self.sequence_namer.setText(self.extract_text_before_brackets(checked_items[0].text()))
-        else:
-            self.unselect_items()
-            self.remove_layout_from_widget(self.parameters_area)
-            
-    def find_checked_items(self, box):
-        checked_items = []
-        for i in range(box.count()):
-            item = box.item(i)
-            if item.checkState() == Qt.Checked:
-                checked_items.append(item)
-        return checked_items
-
-    def remove_sequence(self):
-        selected_sequences = self.find_checked_items(self.listbox4)
-        selected_devices = self.find_checked_items(self.listbox2)
-        # selected_sequences = self.listbox4.selectedItems()
-        # selected_devices = self.listbox2.selectedItems()
-        for item in selected_sequences:
-            row = self.listbox4.row(item)  # Get the row of the item
-            self.listbox4.takeItem(row)
-
-        for seq in selected_sequences:
-            a = seq.text()
-            self.runtime_journal[seq.text()][1] = self.runtime_journal[seq.text()][1] - len(selected_devices) 
-
-        for device in selected_devices:
-            for sequence in selected_sequences:
-                try:
-                    self.yamldict['Devices'][device.text()]['sequences'].remove(sequence.text())
-                    print('Removed sequence '+sequence.text()+' from device '+device.text())
-                except: 
-                    for x in self.deviceobjects:
-                        if x.device_id == device.text():
-                            x.sequences.remove(sequence.text())
-                    print('Removed sequence '+sequence.text()+' from device '+device.text())
-
-    def select_keyword(self, item):
-        keyword = self.device_search.text()
-        for i in range(self.listbox2.count()):
-            if keyword in self.listbox2.item(i).text() and keyword != '':
-                self.listbox2.item(i).setCheckState(Qt.Checked)
-
-    def select_highlighted(self, item):
-
-        for i in range(self.listbox2.count()):
-            if self.listbox2.item(i).isSelected():
-                self.listbox2.item(i).setCheckState(Qt.Checked)
-
     def select_all(self, item):
         for i in range(self.listbox2.count()):
             self.listbox2.item(i).setCheckState(Qt.Checked)
 
-    def unselect_all(self, item):
-        for i in range(self.listbox2.count()):
-            self.listbox2.item(i).setCheckState(Qt.Unchecked)
-
     def setup_device_data_sequences(self):
         listbox3 = QListWidget()
         listbox4 = QListWidget()
 
         device_data_sequences_layout = QVBoxLayout()
         device_data_sequences_layout.addWidget(QLabel("Device Data"))
         device_data_sequences_layout.addWidget(listbox3)
@@ -716,15 +460,15 @@
         file_layout.addWidget(self.checkyaml_button)
         self.layout.addLayout(file_layout)
 
     def yaml_check_open(self):
         fname = QFileDialog.getOpenFileName(self, "Open file")
 
         yaml_check(fname[0])
-
+    
     def create_checklist(self, dict, customflag=False):
         checklist = QListWidget()
         for x in dict:
             item = QListWidgetItem(x)
             item.setFlags(item.flags() | Qt.ItemIsUserCheckable)
             item.setCheckState(Qt.Unchecked)
             checklist.addItem(item)
@@ -741,436 +485,120 @@
             if self.sequences_checklist.item(i) != item:
                 self.sequences_checklist.item(i).setCheckState(Qt.Unchecked)
 
         for i in range(self.customsequences_checklist.count()):
             if self.customsequences_checklist.item(i) != item:
                 self.customsequences_checklist.item(i).setCheckState(Qt.Unchecked)
 
-        self.select_items(item.text().split(' ')[0])
-
         if item.checkState() == Qt.Checked:
             # Get the sequence name
             self.sequence_name0 = item.text()
-
-            self.sequence_name0 = self.sequence_name0.split(' ')[0]
-
-            self.custom_reset_parameters(self.sequence_name0)
-            # Get the path to the sequences directory
-            # cwd = os.getcwd()
-            # d = dirname(abspath(__file__))
-            # # print(d)
-            # d = str(d)
-
-            # attributes = self.yamldict["Sequences"][self.sequence_name0]
-
-            # # class_name = self.find_class_names_in_file(sequence_file)
-
-            # # attributes = self.find_instance_attributes_in_init(sequence_file, class_name[0])
-            # # print(attributes)
-
-            # # Clear the existing layout
-            # self.clear_layout(self.parameters_area.layout())
-
-            # # Delete the existing layout
-            # old_layout = self.parameters_area.layout()
-            # if old_layout is not None:
-            #     del old_layout
-
-            # layout, self.widget_list = self.set_parameters(attributes)
-            # # self.populate_sequence_variables(sequence_file, class_name[0])
-
-            # new_layout = self.parameters_area.layout()
-            # if new_layout is None:  # Only set the new layout if there isn't one already
-            #     self.parameters_area.setLayout(layout)
-
-            # # Set the new layout
-            # self.parameters_area.setLayout(layout)
-
-        else:
-            # Clear the text editor
-            self.unselect_items()
-            self.remove_layout_from_widget(self.parameters_area)
-
-    def custom_reset_parameters(self, sequenceName):
-        # Get the sequence name
-            if 'ida' in sequenceName:
-                showresults = False
-            else:
-                showresults = True
-            self.sequence_name0 = sequenceName
             # Get the path to the sequences directory
             cwd = os.getcwd()
             d = dirname(abspath(__file__))
-            # print(d)
+            #print(d)
             d = str(d)
 
             attributes = self.yamldict["Sequences"][self.sequence_name0]
 
-            sequence_name_og = self.extract_text_in_brackets(sequenceName)[0] + ".py"
-
-            script_dir = Path(__file__).parent.resolve()  # Ensure absolute path
-            # Define the relative path *within your project*
-            rel_path = Path("sequences", self.branch, sequence_name_og)
-            # Combine the script directory with the relative path to get the full path
-            mypath = script_dir / rel_path
-            # Resolve the full path on the system
-            sequence_file = str(mypath.resolve())
-
-            class_name = self.find_class_names_in_file(sequence_file)
-
-            attributes2 = self.find_instance_attributes_in_init(sequence_file, class_name[0])
-
-            for entry in attributes:
-                if entry != 'Runtime':
-                    for entry2 in attributes[entry]:
-                        attributes2[entry][entry2] = attributes[entry][entry2]
-
-            self.attributes = attributes2
-
             # class_name = self.find_class_names_in_file(sequence_file)
 
             # attributes = self.find_instance_attributes_in_init(sequence_file, class_name[0])
-            # print(attributes)
+            #print(attributes)
 
             # Clear the existing layout
             self.clear_layout(self.parameters_area.layout())
 
             # Delete the existing layout
             old_layout = self.parameters_area.layout()
             if old_layout is not None:
                 del old_layout
 
-            layout, self.widget_list = self.set_parameters(attributes2, showresults=showresults)
+            layout, self.widget_list = self.set_parameters(attributes)
             # self.populate_sequence_variables(sequence_file, class_name[0])
 
             new_layout = self.parameters_area.layout()
             if new_layout is None:  # Only set the new layout if there isn't one already
                 self.parameters_area.setLayout(layout)
 
             # Set the new layout
             self.parameters_area.setLayout(layout)
 
-    def reset_parameters(self, sequenceName):
-
-        if 'ida' in sequenceName:
-            showresults = False
         else:
-            showresults = True
-        cwd = os.getcwd()
-        d = str(dirname(abspath(__file__)))
-
-        sequence_name = sequenceName + ".py"
-
-        script_dir = Path(__file__).parent.resolve()  # Ensure absolute path
-        # Define the relative path *within your project*
-        rel_path = Path("sequences", self.branch, sequence_name)
-        # Combine the script directory with the relative path to get the full path
-        mypath = script_dir / rel_path
-        # Resolve the full path on the system
-        sequence_file = str(mypath.resolve())
-
-        #sequence_file = os.path.join(d, "sequences", self.branch, sequence_name)
-
-        class_name = self.find_class_names_in_file(sequence_file)
-
-        self.attributes = self.find_instance_attributes_in_init(
-            sequence_file, class_name[0]
-        )
-
-        # Clear the existing layout
-        self.clear_layout(self.parameters_area.layout())
-
-        # Delete the existing layout
-        old_layout = self.parameters_area.layout()
-        if old_layout is not None:
-            del old_layout
-
-        layout, self.widget_list = self.set_parameters(self.attributes, showresults=showresults)
-        self.results_info = self.attributes["results_info"]
-        # self.populate_sequence_variables(sequence_file, class_name[0])
-
-        new_layout = self.parameters_area.layout()
-        if new_layout is None:  # Only set the new layout if there isn't one already
-            self.parameters_area.setLayout(layout)
-
-        # Set the new layout
-        self.parameters_area.setLayout(layout)
-
-    def extract_text_in_brackets(self, text):
-        results = []
-        start_index = None
-        for i, char in enumerate(text):
-            if char == '(':
-                start_index = i + 1  # Record the index after the opening bracket
-            elif char == ')':
-                if start_index is not None:  
-                    results.append(text[start_index:i])
-                    start_index = None
-        return results
-    
-    def extract_text_before_brackets(self, text):
-        current_word = ""
-        in_brackets = False
-        for char in text:
-            if not in_brackets:
-                if char == '(':
-                    in_brackets = True
-                else:
-                    current_word += char
-        return current_word 
+            # Clear the text editor
+            self.remove_layout_from_widget(self.parameters_area)
 
     def set_sequence(self, item):
-        if self.check_for_multiple_sequence_types(self.sequence_name0):
-            print('Please do not choose sequence types from different stages')
-            return
-        
         parameters = self.get_parameters(self.widget_list)
+        if self.edxcheck:
+            parametersdict = {'variables': parameters['variables'], 'results_info': self.resultsinfo}
 
-        if self.check_bounds(parameters):
-            return
-
-        if '(' in self.sequence_namer.text() or ')' in self.sequence_namer.text():
-            print('Please remove brackets from sequence name and try again')
-            return
-
-        a = self.extract_text_in_brackets(self.sequence_name0)
-        if a != []:
-            self.sequence_name0 = a[0]
-
-        name = self.sequence_namer.text() + "(" + self.sequence_name0 + ")"
-        # if self.branch == 'IDA':
-        #     parametersdict = {
-        #         "variables": parameters["variables"],
-        #         "results_info": self.results_info,
-        #     }
-
-        #     self.yamldict["Sequences"][
-        #         self.sequence_namer.text() + "(" + self.sequence_name0 + ")"
-        #     ] = parametersdict
-        # else:
-        self.yamldict["Sequences"][
+            self.yamldict["Sequences"][
+                self.sequence_namer.text() + "(" + self.sequence_name0 + ")"
+            ] = parametersdict
+        else:
+            self.yamldict["Sequences"][
                 self.sequence_namer.text() + "(" + self.sequence_name0 + ")"
             ] = parameters
 
-        runtime = self.sequence_runtime_check(self.sequence_name0, parameters, name)
-        self.update_custom_sequences(self.customsequences_checklist, self.yamldict["Sequences"])
+        self.update_custom_sequences(
+            self.customsequences_checklist, self.yamldict["Sequences"]
+        )
         print("Added Sequence")
-        print(f'This sequence will take approximately {runtime} seconds to run')
-
-    def check_bounds(self, parameters):
-        variables = parameters['variables']
-        check = False
-
-        for variable in variables:
-            if variable + '_bounds' in self.attributes['variables']:
-                try:
-                    a = variables[variable]
-                    b = self.attributes['variables'][variable + '_bounds'][1]
-                    subcheck = 0
-
-                    if ',' in variables[variable]:
-                        readings = variables[variable].split(',')
-                        for i in range(len(readings)):
-                            subcheck = 0
-                            if isinstance(self.attributes['variables'][variable + '_bounds'][0], list):
-                                for j in range(len(self.attributes['variables'][variable + '_bounds'][0])):
-                                    if float(readings[i]) > float(self.attributes['variables'][variable + '_bounds'][1][j]) or float(readings[i]) < float(self.attributes['variables'][variable + '_bounds'][0][j]):
-                                        subcheck += 1
-                                if subcheck == len(self.attributes['variables'][variable + '_bounds'][0]):
-                                    print('Variable {} entry {} is out of bounds'.format(variable, readings[i]))
-                                    print('Ensure variable is within {} and {} or {} and {}'.format(self.attributes['variables'][variable + '_bounds'][0][0], self.attributes['variables'][variable + '_bounds'][1][0], self.attributes['variables'][variable + '_bounds'][0][1], self.attributes['variables'][variable + '_bounds'][1][1] ))
-
-                                    check = True
-                                    subcheck = 0
-                            else:
-                                if float(readings[i]) > float(self.attributes['variables'][variable + '_bounds'][1]) or float(readings[i]) < float(self.attributes['variables'][variable + '_bounds'][0]):
-                                    print('Variable {} entry {} is out of bounds'.format(variable, readings[i]))
-                                    print('Ensure variable is within {} and {}'.format(self.attributes['variables'][variable + '_bounds'][0], self.attributes['variables'][variable + '_bounds'][1]))
-                                    check = True
-                    else:
-                        if isinstance(self.attributes['variables'][variable + '_bounds'][0], list):
-                            for i in range(len(self.attributes['variables'][variable + '_bounds'][0])):
-                                if float(variables[variable]) > float(self.attributes['variables'][variable + '_bounds'][1][i]) or float(variables[variable]) < float(self.attributes['variables'][variable + '_bounds'][0][i]):
-                                    subcheck += 1
-                            if subcheck == len(self.attributes['variables'][variable + '_bounds'][0]):
-                                print('Variable {} is out of bounds'.format(variable))
-                                print('Ensure variable is within {} and {}'.format(self.attributes['variables'][variable + '_bounds'][0], self.attributes['variables'][variable + '_bounds'][1]))
-
-                                check = True
-                                subcheck = 0
-                        else:
-                            if float(variables[variable]) > float(self.attributes['variables'][variable + '_bounds'][1]) or float(variables[variable]) < float(self.attributes['variables'][variable + '_bounds'][0]):
-                                print('Variable {} is out of bounds'.format(variable))
-                                print('Ensure variable is within {} and {}'.format(self.attributes['variables'][variable + '_bounds'][0], self.attributes['variables'][variable + '_bounds'][1]))
-
-                                check = True
-                except:
-                    print('Bounds check failed for variable {}'.format(variable))
-                    check = True
-        return check
-
-    def sequence_runtime_check(self, sequenceName, parameters, name):
-        wavelength_constant = 0.25
-        smu_constant = 0.5
-
-        sequencetypes = [
-            "wavelength_sweep",
-            "current_sweep",
-            "voltage_sweep",
-            "set_current_wavelength_sweep",
-            "set_voltage_wavelength_sweep",
-            "set_wavelength_current_sweep",
-            "set_wavelength_voltage_sweep",
-            "wavelength_sweep_ida",
-            "current_sweep_ida",
-            "voltage_sweep_ida",
-            "set_current_wavelength_sweep_ida",
-            "set_voltage_wavelength_sweep_ida",
-            "set_wavelength_current_sweep_ida",
-            "set_wavelength_voltage_sweep_ida",
-        ]
-
-        sequence = sequenceName
-        variables = parameters['variables']
-        # print(variables)
-        if sequencetypes[6] in sequence or sequencetypes[13] in sequence:
-
-            runtime = (
-                (
-                    (float(variables["Stop"]) - float(variables["Start"]))
-                    / float(variables["Step"])
-                )
-                * smu_constant
-                * (variables["Wavelengths"].count(",") + 1)
-            )
-        elif sequencetypes[5] in sequence or sequencetypes[12] in sequence:
-            runtime = (
-                (
-                    (float(variables["Stop"]) - float(variables["Start"]))
-                    / float(variables["Step"])
-                )
-                * smu_constant
-                * (variables["Wavelengths"].count(",") + 1)
-            )
-        elif sequencetypes[4] in sequence or sequencetypes[11] in sequence:
-            runtime = (
-                (float(variables["Stop"]) - float(variables["Start"]))
-                / float(variables["Step"])
-                * wavelength_constant
-                * (variables["Voltages"].count(",") + 1)
-            )
-        elif sequencetypes[3] in sequence or sequencetypes[10] in sequence:
-            runtime = (
-                (float(variables["Stop"]) - float(variables["Start"]))
-                / float(variables["Step"])
-                * wavelength_constant
-                * (variables["Currents"].count(",") + 1)
-            )
-        elif sequencetypes[2] in sequence or sequencetypes[9] in sequence:
-            runtime = (
-                (float(variables["Stop"]) - float(variables["Start"]))
-                / float(variables["Step"])
-            ) * smu_constant
-        elif sequencetypes[1] in sequence or sequencetypes[8] in sequence:
-            runtime = (
-                (float(variables["Stop"]) - float(variables["Start"]))
-                / float(variables["Step"])
-            ) * smu_constant
-        elif sequencetypes[0] in sequence or sequencetypes[7] in sequence:
-            runtime = (
-                (float(variables["Stop"]) - float(variables["Start"]))
-                / float(variables["Step"])
-                * wavelength_constant
-            )
-        else:
-            print("Error in predicting runtime. Please check sequence type and parameters.")
-            return None
-        self.runtime_journal[name] = [runtime, 0]
-        self.yamldict["Sequences"][name]['Runtime'] = runtime
-        return runtime
-
-    def total_runtime_check(self, yamldict):
-        """
-        Checks the runtime of all the sequences on all specified devices.
-        """
-
-        sequences = yamldict["Sequences"]
-        devices = yamldict['Devices']
-
-        # for device in devices:
-        #     for sequence in devices[device]['sequences']:
-        #         self.runtime_journal[sequence][1] = self.runtime_journal[sequence][1] + 1
-
-        move_time_constant = 1
-        total_runtime = 0
-
-        for seq in self.runtime_journal:
-            total_runtime = total_runtime + self.runtime_journal[seq][0] * self.runtime_journal[seq][1]
-
-        return total_runtime
-
+        
     def to_title_case(self, s):
-        return "".join(word.capitalize() for word in s.split("_"))
+        return ''.join(word.capitalize() for word in s.split('_'))
 
+        
         self.update_custom_sequences(
             self.customsequences_checklist, self.yamldict["Sequences"]
         )
         print("Added Sequence")
 
-    def choose_file(self):
+    def choose_coord_file(self):
         fname = QFileDialog.getOpenFileName(self, "Open file")
         if fname[0]:
             self.file_label.setText(fname[0])
-            #self.file_label.setText("No file selected")
+            self.yfile_label.setText("No file selected")
+
+        if fname[0].endswith(".yaml") == True:
+            print("Please select a coordinate file not a yaml file")
+
+        if fname[0] != "" and fname[0].endswith(".yaml") == False:
+            try:
+                self.deviceobjects = self.create_devices_from_file(fname[0])
+                self.populate_device_list()
+                self.populate_group_list()
+                self.populate_polar_list()
+                self.populate_wavelength_list()
+            except:
+                print("Errors found in coordinate file, please remove or edit and upload again")
+
+    def choose_yaml_file(self):
+        fname = QFileDialog.getOpenFileName(self, "Open file")
+        if fname[0]:
+            self.yfile_label.setText(fname[0])
+            self.file_label.setText("No file selected")
+
+        if fname[0].endswith(".yaml") == False:
+            print("Please select a yaml file not a coordinate file")
 
         if fname[0] != "" and fname[0].endswith(".yaml") == True:
             with open(fname[0], "r") as file:
                 inputfile = yaml.safe_load(file)
 
-
-            self.yamldict = inputfile
             self.devicedict = inputfile["Devices"]
             self.routinedict = inputfile["Sequences"]
-            self.update_custom_sequences(self.customsequences_checklist, inputfile["Sequences"])
-
 
             self.deviceobjects = self.create_device_list(self.devicedict)
 
             self.populate_device_list()
             self.populate_group_list()
             self.populate_polar_list()
             self.populate_wavelength_list()
-        elif fname[0] != "" and fname[0].endswith(".txt") == True:
-            with open(fname[0], "r") as file:
-                lines = file.readlines()
-            if lines[0] != '% X-coord, Y-coord, Polarization, wavelength, type, deviceID, params \n' and lines[0] != '% X-coord, Y-coord, Polarization, wavelength, type, deviceID, params\n':
-                print("Incorrect format for coordinate file, please reupload with correct format")
-                print('First line should be "% X-coord, Y-coord, Polarization, wavelength, type, deviceID, params"')
-                print('First line is ' + lines[0])
-                self.file_label.setText('No file selected')
-                return
-            try:
-                self.deviceobjects = self.create_devices_from_file(fname[0])
-                self.populate_device_list()
-                self.populate_group_list()
-                self.populate_polar_list()
-                self.populate_wavelength_list()
-            except:
-                print(
-                    "Errors found in coordinate file, please remove or edit and upload again"
-                )
-        else:
-            print("Please select either a valid yaml file or coordinate text file")
-
-    def populateCustomSequences(self, inputfile):
-        self.customsequences_checklist = []
-        if "CustomSequences" in inputfile:
-            custom_sequences = inputfile["CustomSequences"]
-            for sequence in custom_sequences:
-                self.customsequences_checklist.append(sequence["Name"])
 
     # Redefining the function create_devices_from_file with handling blank lines in electrical coordinates data
     def create_devices_from_file(self, file_path):
         """
         This function creates a list of ElectroOpticDevice objects from the input text file.
         Each line in the first part of the text file corresponds to a device.
         The second part of the text file contains the electrical coordinates for the devices.
@@ -1180,23 +608,15 @@
 
         Returns:
             list: A list of ElectroOpticDevice objects.
         """
         # Dictionary to store the created ElectroOpticDevice objects
         devices_dict = {}
         save_location = dirname(abspath(__file__))
-        save_location = (
-            str(save_location)
-            + "\\"
-            + "File_edits"
-            + "\\"
-            + "coordinate_file_edits.txt"
-        )
-
-        optLines, ElecLines = self.countLines(file_path)
+        save_location = str(save_location) + "\\" + 'File_edits' + "\\" + "coordinate_file_edits.txt"
 
         file = self.remove_comments_from_lines(file_path, save_location)
         file = self.account_for_underscores(file, save_location)
         file = self.append_number_to_duplicate_device_ids(file, save_location)
         file = self.check_coordfile_titles(file, save_location)
         errors = self.check_number_of_columns_optical(file)
         file = self.elec_pad_underscore_issue(file, save_location)
@@ -1221,99 +641,69 @@
 
         # Electrical coordinates data is after the blank line and also has a header line
         elec_coords_data = data[blank_line_index + 2 :]
 
         # Create ElectroOpticDevice objects from device data
         for count, line in enumerate(device_data):
             try:
-                x, y, polarization, wavelength, device_type, device_id = line.split(
-                    ", "
-                )
+                x, y, polarization, wavelength, device_type, device_id = line.split(", ")
                 optical_coords = [float(x), float(y)]
                 device = ElectroOpticDevice(
                     device_id, wavelength, polarization, optical_coords, device_type
                 )
                 devices_dict[device_id] = device
             except:
-                print("Error in optical coordinate line: " + str(count + 2) + ": " + line)
+                print("Error in optical coordinate line: " + str(count) + ': '+ line)
 
         # Add electrical coordinates to devices
         for count, line in enumerate(elec_coords_data):
             # Skip blank lines
             if line:
                 try:
                     x, y, device_id, pad_name = line.split(", ")
                     elec_coords = [pad_name, float(x), float(y)]
                     devices_dict[device_id].add_electrical_coordinates(elec_coords)
                 except:
-                    print(
-                        "Error in electrical coordinate line: "
-                        + str(count + optLines + 3)
-                        + ": "
-                        + line
-                    )
+                    print("Error in electrical coordinate line: " + str(count) + ': '+ line)
 
         for devicename in devices_dict:
-            self.yamldict["Devices"][devices_dict[devicename].device_id] = (
-                self.object_to_dict(devices_dict[devicename])
-            )
+            self.yamldict["Devices"][
+                devices_dict[devicename].device_id
+            ] = self.object_to_dict(devices_dict[devicename])
 
         return list(devices_dict.values())
-    
-    def countLines(self, file_path):
-        """
-        This function counts the number of lines in the optical and electrical coordinate files.
-        It also counts the number of optical coordinate lines and the number of electrical coordinate lines.
-        """
-
-        optLines = 0
-        ElecLines = 0
-        optcheck = True
-
-        with open(file_path, "r") as file:
-            lines = file.readlines()
-
-        for line in lines:
-            if line == "\n":  # Check for the line with just '\n'
-                optcheck = False
-            if optcheck == True:
-                optLines += 1
-            else:
-                ElecLines += 1
-    
-        return optLines, ElecLines
 
     def create_device_list(self, devicedict):
         device_list = []
         for device_info in devicedict.values():
             device = ElectroOpticDevice(
-                device_id=device_info["device_id"],
-                opticalCoords=device_info["opticalCoordinates"],
-                polarization=device_info["polarization"],
-                device_type=device_info["device_type"],
-                wavelength=device_info["wavelength"],
+                device_id=device_info["DeviceID"],
+                opticalCoords=device_info["Optical Coordinates"],
+                polarization=device_info["Polarization"],
+                device_type=device_info["Type"],
+                wavelength=device_info["Wavelength"],
             )
-            if device_info["electricalCoordinates"] != []:
-                device.add_electrical_coordinates(device_info["electricalCoordinates"])
-            device.add_sequences(device_info["sequences"])
+            if device_info["Electrical Coordinates"] != []:
+                device.add_electrical_coordinates(device_info["Electrical Coordinates"])
+            device.add_sequences(device_info["Sequences"])
             device_list.append(device)
             self.yamldict["Devices"][device.device_id] = self.object_to_dict(device)
         return device_list
-
+    
     def fix_coord_file(self, item):
         fname = QFileDialog.getOpenFileName(self, "Open file")
         if fname[0]:
             self.file_label.setText(fname[0])
             self.yfile_label.setText("No file selected")
 
         if fname[0].endswith(".yaml") == True:
             print("Please select a coordinate file not a yaml file")
 
         if fname[0] != "" and fname[0].endswith(".yaml") == False:
-            save_location = fname[0].replace(".txt", "_adjusted.txt")
+            save_location = fname[0].replace('.txt', '_adjusted.txt')
 
             file = self.remove_comments_from_lines(fname[0], save_location)
             file = self.account_for_underscores(file, save_location)
             file = self.append_number_to_duplicate_device_ids(file, save_location)
             file = self.check_coordfile_titles(file, save_location)
             errors = self.check_number_of_columns_optical(file)
             file = self.elec_pad_underscore_issue(file, save_location)
@@ -1323,169 +713,161 @@
                 for x in errors:
                     print(x)
 
     def elec_pad_underscore_issue(self, input_file_path, output_file_path):
         modified_lines = []
         process_line = False  # Flag to indicate if the line should be processed
 
-        with open(input_file_path, "r") as file:
+        with open(input_file_path, 'r') as file:
             lines = file.readlines()
 
         for line in lines:
-            if line == "\n":  # Check for the line with just '\n'
+            if line == '\n':  # Check for the line with just '\n'
                 process_line = True
 
             if process_line:
-                if line.strip().startswith("%"):
+                if line.strip().startswith('%'):
                     modified_lines.append(line)
                     continue
-                elements = line.strip().split(", ")
+                elements = line.strip().split(', ')
                 if len(elements) > 4:
-                    # Keep the first, second, and last elements as they are
+                     # Keep the first, second, and last elements as they are
                     # Combine the middle elements with underscores
-                    combined_middle = "_".join(elements[2:-1])
+                    combined_middle = '_'.join(elements[2:-1])
                     elements = elements[:2] + [combined_middle] + elements[-1:]
-                line = ", ".join(elements) + "\n"
+                line = ', '.join(elements) + '\n'
                 modified_lines.append(line)
             else:
                 # Simply append the line as is, without modification
                 modified_lines.append(line)
 
-        with open(output_file_path, "w") as file:
+        with open(output_file_path, 'w') as file:
             file.writelines(modified_lines)
 
         return output_file_path
 
     def account_for_underscores(self, input_file_path, output_file_path):
         modified_lines = []
         process_line = True  # Flag to indicate if the line should be processed
 
-        with open(input_file_path, "r") as file:
+        with open(input_file_path, 'r') as file:
             lines = file.readlines()
 
         for line in lines:
-            if line == "\n":  # Check for the line with just '\n'
+            if line == '\n':  # Check for the line with just '\n'
                 process_line = False
 
             if process_line:
-                if line.strip().startswith("%"):
+                if line.strip().startswith('%'):
                     modified_lines.append(line)
                     continue
-                elements = line.strip().split(", ")
+                elements = line.strip().split(', ')
                 if len(elements) > 6:
-                    elements[5:] = ["_".join(elements[5:])]
-                line = ", ".join(elements) + "\n"
+                    elements[5:] = ['_'.join(elements[5:])]
+                line = ', '.join(elements) + '\n'
                 modified_lines.append(line)
             else:
                 # Simply append the line as is, without modification
                 modified_lines.append(line)
 
-        with open(output_file_path, "w") as file:
+        with open(output_file_path, 'w') as file:
             file.writelines(modified_lines)
 
         return output_file_path
 
-    def check_number_of_columns_optical(
-        self, input_file_path, delimiter=", ", expected_columns=6, comment_char="%"
-    ):
-        alerts = (
-            []
-        )  # List to hold the alerts if any rows have a different number of columns
+    def check_number_of_columns_optical(self, input_file_path, delimiter=', ', expected_columns=6, comment_char='%'):
+        alerts = []  # List to hold the alerts if any rows have a different number of columns
         process_line = True  # Flag to indicate if the line should be processed
-
-        with open(input_file_path, "r") as file:
+        
+        with open(input_file_path, 'r') as file:
             for line_number, line in enumerate(file, start=1):
-                if line == "\n":  # Check for the line with just '\n'
+                if line == '\n':  # Check for the line with just '\n'
                     process_line = False
                 # Skip empty lines and commented lines
                 if process_line:
                     if not line.strip() or line.strip().startswith(comment_char):
                         continue
-
+                    
                     columns = line.strip().split(delimiter)
                     if len(columns) != expected_columns:
                         alerts.append((line_number, line.strip()))
-
+        
         return alerts
 
     def check_coordfile_titles(self, input_file_path, output_file_path):
         # Define the required title lines
-        title_line_1 = (
-            "% X-coord, Y-coord, Polarization, wavelength, type, deviceID, params \n"
-        )
-        title_line_2 = "% X-coord, Y-coord, deviceID, padName, params \n"
-
-        with open(input_file_path, "r") as file:
+        title_line_1 = '% X-coord, Y-coord, Polarization, wavelength, type, deviceID, params \n'
+        title_line_2 = '% X-coord, Y-coord, deviceID, padName, params \n'
+        
+        with open(input_file_path, 'r') as file:
             lines = file.readlines()
 
         # Check if the first line matches the required title line 1
         if lines[0].strip() != title_line_1.strip():
             lines.insert(0, title_line_1)
-
+        
         # Check if the title line 2 exists anywhere in the file
         if title_line_2 not in lines:
-            lines.append(
-                "\n"
-            )  # Ensure there is a newline before appending the title line 2
+            lines.append('\n')  # Ensure there is a newline before appending the title line 2
             lines.append(title_line_2)
 
         # Write the modified lines to the output file
-        with open(output_file_path, "w") as file:
+        with open(output_file_path, 'w') as file:
             file.writelines(lines)
 
         return output_file_path
 
     def remove_comments_from_lines(self, input_file_path, output_file_path):
         # This function will remove the word "comment" from the end of each line
         modified_lines = []
 
-        with open(input_file_path, "r") as file:
+        with open(input_file_path, 'r') as file:
             lines = file.readlines()
 
         for line in lines:
             # Check if 'comment' is at the end of the line (considering possible trailing spaces)
-            if "comment" in line:
+            if 'comment' in line:
                 # Remove the word 'comment' (and surrounding whitespace)
-                line = line.replace(", comment", "").rstrip() + "\n"
+                line = line.replace(', comment', '').rstrip() + '\n'
             modified_lines.append(line)
 
         # Write the modified lines to the output file
-        with open(output_file_path, "w") as file:
+        with open(output_file_path, 'w') as file:
             file.writelines(modified_lines)
 
         return output_file_path
-
+        
     def append_number_to_duplicate_device_ids(self, input_file_path, output_file_path):
         device_id_counter = {}
         modified_lines = []
 
-        with open(input_file_path, "r") as file:
+        with open(input_file_path, 'r') as file:
             lines = file.readlines()
 
         for line in lines:
-            if not line.startswith("%"):  # ignore comment lines
-                parts = line.split(", ")
-
+            if not line.startswith('%'):  # ignore comment lines
+                parts = line.split(', ')
+                    
                 device_id = parts[-1].strip()  #
                 # Check if the device_id has already been encountered
                 if device_id in device_id_counter:
-                    # Increment the count and append it to the device_id
+                # Increment the count and append it to the device_id
                     device_id_counter[device_id] += 1
                     new_device_id = f"{device_id}_{device_id_counter[device_id]}"
-                    parts[-1] = new_device_id + "\n"  # replace with the new_device_id
+                    parts[-1] = new_device_id + '\n'  # replace with the new_device_id
                 else:
                     # Initialize the count for this device_id
                     device_id_counter[device_id] = 0
                 # Reconstruct the line
-                line = ", ".join(parts)
+                line = ', '.join(parts)
             # Add the (possibly modified) line to the list of modified lines
             modified_lines.append(line)
 
         # Write the modified lines to the output file
-        with open(output_file_path, "w") as file:
+        with open(output_file_path, 'w') as file:
             file.writelines(modified_lines)
 
         return output_file_path
 
     def update_device_list(self, item):
         # Clear the device listbox before populating
         self.listbox2.clear()
@@ -1496,42 +878,31 @@
         checked_device_nm = set()
 
         # Iterate over all items in the group listbox and add the checked ones to the set
         for i in range(self.listbox1.count()):
             if self.listbox1.item(i).checkState() == Qt.Checked:
                 checked_device_types.add(self.listbox1.item(i).text())
 
-
         for i in range(self.listbox1_2.count()):
             if self.listbox1_2.item(i).checkState() == Qt.Checked:
                 checked_device_polarization.add(self.listbox1_2.item(i).text())
 
-
         for i in range(self.listbox1_3.count()):
             if self.listbox1_3.item(i).checkState() == Qt.Checked:
                 checked_device_nm.add(self.listbox1_3.item(i).text())
 
+        
+
         # Iterate over all devices and add those of the checked types to the device listbox
         for device in self.deviceobjects:
-            check = True
-                
-            if checked_device_types and device.device_type not in checked_device_types:
-                check = False 
-
-            if checked_device_polarization and device.polarization not in checked_device_polarization:
-                check = False
-
-            if checked_device_nm and device.wavelength not in checked_device_nm:
-                check = False
-
-            if check == True:
+            if device.device_type in checked_device_types and device.polarization in checked_device_polarization and device.wavelength in checked_device_nm:
                 device_item = QListWidgetItem(device.device_id)
                 device_item.setFlags(device_item.flags() | Qt.ItemIsUserCheckable)
                 device_item.setCheckState(Qt.Unchecked)
-                self.listbox2.addItem(device_item) 
+                self.listbox2.addItem(device_item)
 
         # Connect the itemChanged signal to the update_device_data slot
         self.listbox2.itemChanged.connect(self.update_device_data)
 
     def populate_device_list(self):
         # Clear listbox2 before populating
         self.listbox2.clear()
@@ -1612,17 +983,15 @@
 
     def rearrange_list_items(self, list_widget: QListWidget, search_string: str):
         matching_items = []
         non_matching_items = []
 
         # Temporarily store items and detach them from the list
         for index in range(list_widget.count()):
-            item = list_widget.takeItem(
-                0
-            )  # Take the first item (since the list is being shortened each time)
+            item = list_widget.takeItem(0)  # Take the first item (since the list is being shortened each time)
             if search_string.lower() in item.text().lower():
                 matching_items.append(item)
             else:
                 non_matching_items.append(item)
 
         # Add the items back to the list in the new order
         for item in matching_items + non_matching_items:
@@ -1661,18 +1030,17 @@
                     )
 
                     # Populate the device data listbox with the formatted device data
                     device_data_item = QListWidgetItem(device_data_str)
                     self.listbox3.addItem(device_data_item)
 
                     # Populate the associated sequences listbox with the sequences associated with the device
-                    for i, sequence in enumerate(device.sequences):
+                    for sequence in device.sequences:
                         sequence_item = QListWidgetItem(sequence)
                         self.listbox4.addItem(sequence_item)
-                        self.listbox4.item(i).setCheckState(Qt.Unchecked)
 
     def choose_save_file(self):
         fname = QFileDialog.getOpenFileName(self, "Open file")
         if fname[0]:
             self.file_label.setText(fname[0])
 
         with open(fname[0], "r") as file:
@@ -1714,16 +1082,46 @@
             if self.customsequences_checklist.item(i) != item:
                 self.customsequences_checklist.item(i).setCheckState(Qt.Unchecked)
         # Check if the item is checked
         if item.checkState() == Qt.Checked:
             # Get the sequence name
             self.sequence_name0 = item.text()
             # Get the path to the sequences directory
-            self.reset_parameters(self.sequence_name0)
-            
+            cwd = os.getcwd()
+            d = str(dirname(abspath(__file__)))
+
+            sequence_name = self.sequence_name0 + ".py"
+
+            sequence_file = os.path.join(d, 'sequences', sequence_name)
+
+            class_name = self.find_class_names_in_file(sequence_file)
+
+            attributes = self.find_instance_attributes_in_init(
+                sequence_file, class_name[0]
+            )
+
+            # Clear the existing layout
+            self.clear_layout(self.parameters_area.layout())
+
+            # Delete the existing layout
+            old_layout = self.parameters_area.layout()
+            if old_layout is not None:
+                del old_layout
+
+            layout, self.widget_list = self.set_parameters(attributes)
+            self.resultsinfo = attributes['resultsinfo']
+            # self.populate_sequence_variables(sequence_file, class_name[0])
+
+            new_layout = self.parameters_area.layout()
+            if new_layout is None:  # Only set the new layout if there isn't one already
+                self.parameters_area.setLayout(layout)
+
+            # Set the new layout
+            self.parameters_area.setLayout(layout)
+
         else:
             # Clear the text editor
             self.remove_layout_from_widget(self.parameters_area)
 
     def remove_layout_from_widget(self, widget):
         old_layout = widget.layout()
         if old_layout is not None:
@@ -1749,88 +1147,70 @@
                     current_sub_dict = {}
                 current_main_key = widget.text()
 
             elif isinstance(widget, tuple) and len(widget) == 3:
                 # This is a sub-dictionary key-value pair
                 key_widget, value_widget, buttton_widget = widget
                 key = key_widget.text()
-                if isinstance(value_widget, QLineEdit):
-                    value = value_widget.text()
-                elif isinstance(value_widget, QComboBox):
-                    value = value_widget.currentText()
+                value = value_widget.text()
                 current_sub_dict[key] = value
 
         # Add the last sub-dictionary
         if current_main_key:
             result_dict[current_main_key] = current_sub_dict
 
         return result_dict
 
-    def check_for_multiple_sequence_types(self, name):
-
-        for i in range(self.customsequences_checklist.count()):
-            if 'ida' in self.customsequences_checklist.item(i).text() and 'ida' not in name:
-                return True
-            else:
-                return False
-        return False
-
-    def set_parameters(self, main_dict, showresults=True):
+    def set_parameters(self, main_dict):
         # Initialize a list to hold the created QLabel and QLineEdit widgets
         widgets_list = []
 
         # Initialize a layout to organize the widgets
         layout = QFormLayout()
         variables_layout = QFormLayout()
         results_info_layout = QFormLayout()
 
         # Loop through the keys of the main dictionary
         for name in main_dict.keys():
             # Create a QLabel with the given name
             dict_label = QLabel(name)
 
             # Add the QLabel to the layout and widget list
-            if showresults:# and dict_label.text() != "results_info":
-                layout.addRow(dict_label)
+            layout.addRow(dict_label)
             widgets_list.append(dict_label)
 
+    
             # Loop through the keys of the sub-dictionary
             for key in main_dict[name].keys():
                 # Create QLabel and QLineEdit for each key
-                if "_info" not in key and "_bounds" not in key and "_options" not in key:
+                if '_info' not in key:
                     key_label = QLabel(str(key))
-                    if key + "_info" in main_dict[name].keys():
-                        key_info = PopupButton("?", main_dict[name][key + "_info"])
+                    key_edit = QLineEdit(str(main_dict[name][key]))
+                    if key + '_info' in main_dict[name].keys():
+                        key_info = PopupButton('?', main_dict[name][key + '_info'])
                     else:
                         key_info = None
 
-                    if key + "_options" in main_dict[name].keys():
-                        key_edit = QComboBox()
-                        key_edit.addItems(main_dict[name][key + "_options"])
-                        key_edit.setCurrentText(main_dict[name][key]) 
-                    else:
-                        key_edit = QLineEdit(str(main_dict[name][key]))
-
                     # Create a horizontal layout for the row
                     row_layout = QHBoxLayout()
-
-                    if (
-                        name == "results_info" and self.branch != 'IDA'
-                    ) or name == "variables":
+                        
+                    if (name == 'resultsinfo' and self.edxcheck == False) or name == 'variables':
                         # Add the label and line edit to the row layout
                         row_layout.addWidget(key_label)
                         row_layout.addWidget(key_edit)
 
                         # Add the button to the row layout if it exists
                         if key_info is not None:
                             row_layout.addWidget(key_info)
 
                         # Add the row layout to the main form layout
                         layout.addRow(row_layout)
 
+                    
+
                     # Add the QLabel and QLineEdit to the layout and widget list
 
                     # if key_info is not None:
                     #     layout.addRow(key_label, key_edit, key_info)
                     # else:
                     #     layout.addRow(key_label, key_edit)
                     widgets_list.append((key_label, key_edit, key_info))
@@ -1846,29 +1226,29 @@
         spec.loader.exec_module(sequence_module)
 
         # Assuming the class name in the sequence file is 'SequenceClass'
 
         sequence_class = getattr(sequence_module, class_name)
         sequence_class1 = sequence_module.VoltageSweep()
 
-        # Accessing the variables and results_Info dictionaries
+        # Accessing the variables and resultsInfo dictionaries
         variables = (
             sequence_class.variables if hasattr(sequence_class, "variables") else {}
         )
-        results_Info = (
-            sequence_class.results_Info if hasattr(sequence_class, "results_Info") else {}
+        resultsInfo = (
+            sequence_class.resultsInfo if hasattr(sequence_class, "resultsInfo") else {}
         )
 
         # Updating the QTextEdit area for sequence variables
         self.sequence_variables_textedit.clear()
         self.sequence_variables_textedit.append("Variables:")
         for key, value in variables.items():
             self.sequence_variables_textedit.append(f"{key}: {value}")
         self.sequence_variables_textedit.append("\\nResults Info:")
-        for key, value in results_Info.items():
+        for key, value in resultsInfo.items():
             self.sequence_variables_textedit.append(f"{key}: {value}")
 
     def clear_layout(self, layout):
         if layout is not None:
             while layout.count():
                 item = layout.takeAt(0)
                 widget = item.widget()
@@ -1898,30 +1278,24 @@
             tree = ast.parse(f.read())
 
         instance_attributes = {}
 
         def handle_expression(expr):
             if isinstance(expr, ast.Str):  # String value
                 return expr.s
-            elif isinstance(expr, ast.Constant):  # Use ast.Constant for numbers
-                if isinstance(expr.value, int) or isinstance(expr.value, float):  # Check for numbers
-                    return expr.value 
+            elif isinstance(expr, ast.Constant):  # Use ast.Constant for numbers 
+                return expr.value  # Access the value directly
             elif isinstance(expr, ast.Name):  # Variable or other reference
                 return expr.id
             elif isinstance(expr, ast.NameConstant):  # Boolean or None value
                 return expr.value
             elif isinstance(expr, ast.Dict):  # Dictionary
                 keys = [handle_expression(k) for k in expr.keys]
                 values = [handle_expression(v) for v in expr.values]
                 return {key: value for key, value in zip(keys, values)}
-            elif isinstance(expr, ast.List): # List
-                return [handle_expression(element) for element in expr.elts]
-            elif isinstance(expr, ast.UnaryOp) and isinstance(expr.op, ast.USub):  # Negative sign
-                if isinstance(expr.operand, ast.Constant):  # Check if operand is a number
-                    return -expr.operand.value     # Return negative of the constant
             else:
                 return "complex_expression"  # Placeholder for more complex expressions
 
         # def handle_expression(expr):
         #     if isinstance(expr, ast.Str):  # String value
         #         return expr.s
         #     elif isinstance(expr, ast.Num):  # Numeric value
@@ -1952,35 +1326,33 @@
                                         and isinstance(target.value, ast.Name)
                                         and target.value.id == "self"
                                     ):
                                         attribute_name = target.attr
                                         attribute_value = handle_expression(
                                             init_node.value
                                         )
-                                        instance_attributes[attribute_name] = (
-                                            attribute_value
-                                        )
+                                        instance_attributes[
+                                            attribute_name
+                                        ] = attribute_value
 
         return instance_attributes
 
-
 class StreamRedirector(object):
     def __init__(self, widget, file=None):
         self.widget = widget
         self.file = file
 
     def write(self, text):
         self.widget.append(text)  # Append text to the QTextEdit widget
         if self.file:
             self.file.write(text)  # Optionally write to a file
 
     def flush(self):
         pass
 
-
 class PopupButton(QPushButton):
     def __init__(self, title, popup_message):
         super().__init__(title)
         self.popup_message = popup_message
         self.clicked.connect(self.showPopup)
         size = 20
         self.setFixedSize(size, size)
@@ -1988,42 +1360,36 @@
     def showPopup(self):
         msg = QMessageBox()
         msg.setWindowTitle("Info")
         msg.setText(self.popup_message)
         msg.setIcon(QMessageBox.Information)
         msg.exec_()
 
-
 class LogEmitter(QObject):
-    """Custom signal emitter for log messages."""
-
+    """ Custom signal emitter for log messages. """
     emitLog = pyqtSignal(str)
 
-
 class StreamToLogger:
     """
     Custom stream object that redirects writes to a logger instance.
     """
-
     def __init__(self, logger, level):
         self.logger = logger
         self.level = level
 
     def write(self, message):
         # Avoid writing newline characters
-        if message != "\n":
+        if message != '\n':
             self.logger.log(self.level, message)
 
     def flush(self):
         pass
 
-
 class QTextEditLogger(logging.Handler, QObject):
-    """Custom logging handler sending log messages to a QTextEdit."""
-
+    """ Custom logging handler sending log messages to a QTextEdit. """
     def __init__(self, parent):
         super().__init__()
         QObject.__init__(self)
         self.widget = QTextEdit(parent)
         self.widget.setReadOnly(True)
         self.logEmitter = LogEmitter()
         self.logEmitter.emitLog.connect(self.appendLogMessage)
@@ -2031,15 +1397,14 @@
     def emit(self, record):
         msg = self.format(record)
         self.logEmitter.emitLog.emit(msg)
 
     def appendLogMessage(self, message):
         self.widget.append(message)
 
-
 class ElectroOpticDevice:
     """Object used to store all information associated with an electro-optic device
 
     Args:
         device_id (str): name of the device
         wavelength(int): wavelength for measuring the device
         polarization(str): 'TE' or 'TM'
@@ -2055,15 +1420,15 @@
         self.device_type = device_type
         self.electricalCoordinates = []
         self.sequences = []
         # self.results = Results()
 
     def add_electrical_coordinates(self, elecCoords):
         """Associates a bondpad with the device"""
-        self.electricalCoordinates = elecCoords
+        self.electricalCoordinates.append(elecCoords)
 
     def get_optical_coordinates(self):
         """Returns the coordinates of the optical input for the device as [x coordinate, y coordinate]"""
         if self.opticalCoordinates:
             return self.opticalCoordinates
 
     def get_electrical_coordinates(self):
@@ -2126,15 +1491,14 @@
             bool: True if the device has routines, False if not.
         """
         if self.routines:
             return True
         else:
             return False
 
-
 class DirectoryDict:
     def __init__(self, directory):
         self.directory = directory
         self.dir_dict = self.create_dict_from_dir()
         self.observer = Observer()
         self.handler = self.DirectoryHandler(self)
         self.observer.schedule(self.handler, self.directory, recursive=True)
@@ -2170,14 +1534,15 @@
                     file_name_without_extension = os.path.splitext(file)[0]
                     module_name = file_name_without_extension
                     module_path = os.path.join(root, file)
                     spec = importlib.util.spec_from_file_location(
                         module_name, module_path
                     )
                     module = importlib.util.module_from_spec(spec)
+                    spec.loader.exec_module(module)
                     classes = [
                         m[1]
                         for m in inspect.getmembers(
                             module,
                             lambda m: inspect.isclass(m)
                             and m.__module__ == module.__name__,
                         )
@@ -2188,15 +1553,14 @@
     class DirectoryHandler(FileSystemEventHandler):
         def __init__(self, dir_dict):
             self.dir_dict = dir_dict
 
         def on_modified(self, event):
             self.dir_dict.dir_dict = self.dir_dict.create_dict_from_dir()
 
-
 if __name__ == "__main__":
     app = QApplication([])
     ex = GUI()
     ex.show()
     app.exec_()
 
 # %%
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/current_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,46 +7,39 @@
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
         self.variables = {
             'Start': 0, 
             'Start_info': 'Please enter the starting current value',
-            'Start_bounds': [-100, 100],
             'Stop': 1,
             'Stop_info': 'Please enter the stopping current value', 
-            'Stop_bounds': [-100, 100],
             'Step': 0.1, 
             'Step_info': 'Please enter the step size',
-            'Step_bounds': [-100, 100],
             'Center': '',
             'Center_info': 'Please enter the center current value',
-            'Center_bounds': [-100, 100],
             'Span': '',
             'Span_info': 'Please enter the span of the sweep',
             'Range': '',
             'Range_info': 'Please enter the range of the sweep',
             'Spacing': '',
             'Spacing_info': 'Please enter the spacing of the sweep',
             'Points': '',
             'Points_info': 'Please enter the number of points in the sweep',
             'Direction': 'UP',
             'Direction_info': 'Please enter the direction of the sweep',
-            'Direction_options': ['UP', 'DOWN'],
             'Sweeptype': 'current',
             'Sweeptype_info': 'Please enter the sweep type should be set to current',
             'Upper_limit': 5,
             'Upper_limit_info': 'Please enter the upper limit of the sweep',
-            'Upper_limit_bounds': [-20, 10],
-            'Trans_col': 'False',
-            'Trans_col_info': 'Please enter True or False for the transient column',
-            'Trans_col_options': ['True', 'False']
+            'Trans_col': False,
+            'Trans_col_info': 'Please enter True or False for the transient column'
         }
 
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
             'plottitle': 'Current Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Current (A)',
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_current_wavelength_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep_ida.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,76 @@
 from dreamcreator.sequences.core.laser_sweep import LaserSweep
 
-class SetCurrentWavelengthSweep(LaserSweep):
+class SetVoltageWavelengthSweepIda(LaserSweep):
     """
-    Sets the current and then performs a laser sweep.
+    Sets the voltage and then performs a laser sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
 
         self.variables = {
-            'Start': 1280,
+            'Start': 1480,
             'Start_info': 'unit nm',
-            'Start_bounds': [[1270, 1480], [1350, 1580]],
-            'Stop': 1370,
+            'Stop': 1580,
             'Stop_info': 'unit nm',
-            'Stop_bounds': [[1270, 1480], [1350, 1580]],
             'Step': 1,
             'Step_info': 'unit nm, can also use wavl_pts, if both filled Step will take priority',
-            'Step_bounds': [[1270, 1480], [1350, 1580]],
-            'wavl_pts': 601,
-            'wavl_pts_info': 'can also use Step, if both filled Step will take priority',
-            'wavl_pts_bounds': [1, 10000],
             'Power': 1,
             'Power_info': 'unit dBm',
-            'Power_bounds': [-70, 10],
-            'Sweep Speed': 20,
-            'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this',
-            'Upper Limit': 0,
-            'Upper Limit_info': 'set to 0',
-            'Upper Limit_bounds': [-30, 10],
-            'Mode': 'CONT',
-            'Mode_info': 'choose between CONT and STEP',
-            'Mode_options': ['CONT', 'STEP'],
+            'Sweep Speed': 'auto',
+            'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this, options are 20nm, 10nm, auto',
             'Laser Output': 'High Power',
-            'Laser Output_info': 'choose between High Power and Low SSE',
-            'Laser_options': ['High Power', 'Low SSE'],
+            'Laser Output_info': 'Set to High Power or Low SSE',
             'Numscans': 1,
             'Numscans_info': 'choose how many scans for each device, default 1, max 3',
-            'Numscans_bounds': [1,3],
             'RangeDec': 20,
             'RangeDec_info': 'default 20',
-            'RangeDec_bounds': [0, 100],
-            'Currents': '0, 1, 2',
-            'Currents_info': 'Please format the currents as a list of integers separated by commas ex. 0, 1, 2',
-            'Currents_bounds': [-30, 30]
+            'Initialrange': '-20',
+            'Initialrange_info': 'default -20',
+            'Channel A': 'True',
+            'Channel A_info': 'Please enter True to use Channel A if not enter False',
+            'Channel B': 'False',
+            'Channel B_info': 'Please enter True to use Channel B if not enter False',
+            'Voltages': '0, 1, 2',
+            'Voltages_info': 'Please enter voltages in units (V) in the form x1, x2, x3',
         }
-        self.results_info = {
+        
+
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
-            'plottitle': 'Set Current Wavelength Sweep',
+            'plottitle': 'Set Voltage Wavelength Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Wavelength (nm)',
             'ytitle': 'Power (dBm)',
             'xscale': 1,
             'yscale': 1,
             'legend': True,
             'csv': True,
             'pdf': True,
             'mat': True,
             'pkl': False
         }
-
         super().__init__(variables=self.variables, resultsinfo=self.resultsinfo, ps=ps)
 
     def run(self, routine=False):
         self.set_results(variables=self.variables, resultsinfo = self.resultsinfo, routine=routine)
+        """Executes a wavelength sweep for each given voltage."""
 
         settings = self.ps.get_settings(self.verbose)
-
-        for current in self.currents:
-            self.ps.elecprobe.smuchannels[0].set_voltage_mode()
-            self.ps.elecprobe.smuchannels[0].set_current(current)
+        
+        for volt in self.variables['voltages']:
+            self.ps.elecprobe.smuchannels[0].set_current_mode()
+            self.ps.elecprobe.smuchannels[0].set_voltage(volt)
             self.ps.elecprobe.smuchannels[0].set_output(True)
         
+            self.external_parameters = volt
+            self.external_unit = 'V'
             self.execute()
 
             self.ps.elecprobe.smuchannels[0].set_output(False)
 
-        self.ps.set_settings(settings)
-
+        self.ps.set_settings(settings)
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_voltage_wavelength_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,67 @@
 from dreamcreator.sequences.core.laser_sweep import LaserSweep
 
-class SetVoltageWavelengthSweep(LaserSweep):
+class SetCurrentWavelengthSweep(LaserSweep):
     """
-    Sets the voltage and then performs a laser sweep.
+    Sets the current and then performs a laser sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
 
         self.variables = {
-            'Start': 1280,
-            'Start_info': 'unit nm',
-            'Start_bounds': [1200, 1400],
-            'Stop': 1370,
-            'Stop_info': 'unit nm',
-            'Stop_bounds': [1200, 1400],
+            'Start': 1480,
+            'Start_info': 'Please enter the start wavelength in nm',
+            'Stop': 1580,
+            'Stop_info': 'Please enter the stop wavelength in nm',
             'Step': 1,
-            'Step_info': 'unit nm, can also use wavl_pts, if both filled Step will take priority',
-            'Step_bounds': [1200, 1400],
-            'wavl_pts': 601,
-            'wavl_pts_info': 'can also use Step, if both filled Step will take priority',
-            'wavl_pts_bounds': [1200, 1400],
+            'Step_info': 'Please enter the step size in nm',
+            'wavl_pts': 101,
+            'wavl_pts_info': 'Please enter the number of wavelength points',
             'Power': 1,
-            'Power_info': 'unit dBm',
-            'Power_bounds': [1200, 1400],
+            'Power_info': 'Please enter the power in dBm',
             'Sweep Speed': 20,
             'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this',
             'Upper Limit': 0,
-            'Upper Limit_info': 'set to 0',
-            'Upper Limit_bounds': [-30, 0],
+            'Upper Limit_info': 'Set to 0',
             'Mode': 'CONT',
-            'Mode_info': 'choose between CONT and STEP',
-            'Mode_options': ['CONT', 'STEP'],
-            'Laser Output': 'High Power',
-            'Laser Output_info': 'choose between High Power and Low SSE',
-            'Laser_options': ['High Power', 'Low SSE'],
-            'Numscans': 1,
-            'Numscans_info': 'choose how many scans for each device, default 1, max 3',
-            'Numscans_bounds': [1,3],
-            'RangeDec': 20,
-            'RangeDec_info': 'default 20',
-            'RangeDec_bounds': [0, 100],
-            'Voltages': '[0, 1, 2]',
-            'Voltages_info': 'Please format the voltages as a list of integers separated by commas ex. [0,1,2]',
-            'Voltages_bounds': [-30, 30]
+            'Mode_info': 'Choose between CONT and STEP',
+            'Currents': '[0,1,2]',
+            'Currents_info': 'Please format the currents as a list of integers separated by commas ex. [0,1,2]'
         }
-
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
-            'plottitle': 'Set Voltage Wavelength Sweep',
+            'plottitle': 'Set Current Wavelength Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Wavelength (nm)',
             'ytitle': 'Power (dBm)',
             'xscale': 1,
             'yscale': 1,
             'legend': True,
             'csv': True,
             'pdf': True,
             'mat': True,
             'pkl': False
         }
+
         super().__init__(variables=self.variables, resultsinfo=self.resultsinfo, ps=ps)
 
     def run(self, routine=False):
         self.set_results(variables=self.variables, resultsinfo = self.resultsinfo, routine=routine)
-        """Executes a wavelength sweep for each given voltage."""
 
         settings = self.ps.get_settings(self.verbose)
-        
-        for volt in self.variables['voltages']:
-            self.ps.elecprobe.smuchannels[0].set_current_mode()
-            self.ps.elecprobe.smuchannels[0].set_voltage(volt)
+
+        for current in self.currents:
+            self.ps.elecprobe.smuchannels[0].set_voltage_mode()
+            self.ps.elecprobe.smuchannels[0].set_current(current)
             self.ps.elecprobe.smuchannels[0].set_output(True)
         
-            self.external_parameters = volt
-            self.external_unit = 'V'
             self.execute()
 
             self.ps.elecprobe.smuchannels[0].set_output(False)
 
-        self.ps.set_settings(settings)
+        self.ps.set_settings(settings)
+
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_wavelength_current_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,49 +6,38 @@
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
 
         self.variables = {
-            'Start': 0, 
-            'Start_info': 'Please enter start voltage (V)',
-            'Start_bounds': [-10, 10],
+            'Start': 0,
+            'Start_info': 'Please enter start value',
             'Stop': 1, 
-            'Stop_info': 'Please enter stop voltage (V)',
-            'Stop_bounds': [-10, 10],
+            'Stop_info': 'Please enter stop value',
             'Step': 0.1, 
-            'Step_info': 'Please enter stepsize (V)',
-            'Step_bounds': [-10, 10],
+            'Step_info': 'Please enter step value',
             'Center': '',
-            'Center_info': 'Please enter center voltage',
-            'Center_bounds': [0, 100],
+            'Center_info': 'Please enter center value',
             'Span': '',
-            'Span_info': 'Please enter span voltage',
-            'Span_bounds': [0, 100],
+            'Span_info': 'Please enter span value',
             'Range': '',
-            'Range_info': 'Please enter range voltage',
-            'Range_bounds': [0, 100],
+            'Range_info': 'Please enter range value',
             'Spacing': '',
-            'Spacing_info': 'Please enter spacing voltage',
-            'Spacing_bounds': [0, 100],
+            'Spacing_info': 'Please enter spacing value',
             'Points': '',
-            'Points_info': 'Please enter points voltage',
-            'Points_bounds': [0, 1000],
+            'Points_info': 'Please enter points value',
             'Direction': 'UP',
-            'Direction_info': 'Please enter direction voltage',
-            'Direction_options': ['UP', 'DOWN'],
+            'Direction_info': 'Please enter direction value',
             'Sweeptype': 'current',
             'Sweeptype_info': 'Please enter sweep type',
-            'Sweeptype_options': ['current'],
             'Wavelengths': [1480, 1500, 1580],
-            'Wavelengths_info': 'Please enter wavelengths value',
-            'Wavelengths_bounds': [[1270, 1480], [1350, 1580]]
+            'Wavelengths_info': 'Please enter wavelengths value'
         }
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
             'plottitle': 'Set Wavelength Current Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Current (A)',
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/set_wavelength_voltage_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep_ida.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,69 @@
 from dreamcreator.sequences.core.smu_sweep import SmuSweep
-import time
 
-class SetWavelengthVoltageSweep(SmuSweep):
+class SetWavelengthCurrentSweepIda(SmuSweep):
     """
-    Sets the wavelength then performs a voltage sweep.
+    Sets the wavelength then performs a current sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
+
         self.variables = {
             'Start': 0, 
-            'Start_info': 'Please enter start voltage (V)',
-            'Start_bounds': [-100, 100],
+            'Start_info': 'Please enter start current (V)',
             'Stop': 1, 
-            'Stop_info': 'Please enter stop voltage (V)',
-            'Stop_bounds': [-100, 100],
-            'Step': 0.1, 
-            'Step_info': 'Please enter stepsize (V)',
-            'Step_bounds': [0.01, 100],
-            'Center': '',
-            'Center_info': 'Please enter center voltage',
-            'Center_bounds': [0, 100],
-            'Span': '',
-            'Span_info': 'Please enter span voltage',
-            'Span_bounds': [0, 100],
-            'Range': '',
-            'Range_info': 'Please enter range voltage',
-            'Range_bounds': [0, 100],
-            'Spacing': '',
-            'Spacing_info': 'Please enter spacing voltage',
-            'Spacing_bounds': [0, 100],
-            'Points': '',
-            'Points_info': 'Please enter points voltage',
-            'Points_bounds': [0, 1000],
-            'Direction': 'UP',
-            'Direction_info': 'Please enter direction voltage',
-            'Direction_options': ['UP', 'DOWN'],
-            'Sweeptype': 'voltage',
-            'Sweeptype_info': 'Please enter sweep type',
-            'Sweeptype_options': ['voltage'],
-            'Upper Limit': 5,
-            'Upper Limit_info': 'Please enter upper limit value',
-            'Upper Limit_bounds': [0, 100],
-            'Trans_col': False,
-            'Trans_col_info': 'Please enter trans_col value',
-            'Trans_col_options': ['True', 'False'],
-            'Wavelengths': [1480, 1500, 1580],
-            'Wavelengths_info': 'Please enter wavelengths value',
-            'Wavelengths_bounds': [[1270, 1480], [1350, 1580]],
-            'Power': 1,
-            'Power_info': 'Please enter power (dBm) value',
-            'Power_bounds': [-70, 100]
+            'Stop_info': 'Please enter stop current (V)',
+            'Res': 0.1, 
+            'Res_info': 'Please enter step current (V)',
+            'IV': 'True',
+            'IV_info': 'True if current vs voltage plot needed',
+            'RV': 'True',
+            'RV_info': 'True if resistance vs voltage plot needed',
+            'PV': 'True',
+            'PV_info': 'True if power vs voltage plot needed',
+            'Channel A': 'True',
+            'Channel A_info': 'Please enter True to use Channel A if not enter False',
+            'Channel B': 'False',
+            'Channel B_info': 'Please enter True to use Channel B if not enter False',
+            'Wavelengths': '1480, 1550, 1580',
+            'Wavelengths_info': 'Set wavelengths in form x, x1, x2 with unit nm'
         }
-        self.results_info = {
+
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
-            'plottitle': 'Set Wavelength Voltage Sweep',
+            'plottitle': 'Set Wavelength Current Sweep',
             'save_location': '',
             'foldername': '',
-            'xtitle': 'Voltage (V)',
-            'ytitle': 'Current (A)',
+            'xtitle': 'Current (A)',
+            'ytitle': 'Voltage (V)',
             'xscale': 1,
             'yscale': 1,
             'legend': True,
             'csv': True,
             'pdf': True,
             'mat': True,
             'pkl': False
         }
 
-        super().__init__(variables=self.variables, resultsinfo=self.resultsinfo, sweeptype='voltage', ps=ps)
+        super().__init__(variable=self.variables, resultsinfo=self.resultsinfo, type='current', ps=ps)
 
     def run(self, routine=False):
         self.set_results(variables=self.variables, resultsinfo = self.resultsinfo, routine=routine)
 
         settings = self.ps.get_settings(self.verbose)
 
-        for wav in self.variables['wavelengths']:
+        for wav in self.wavelengths:
             self.ps.optprobe.laser.set_wavl(wav)
             self.ps.optprobe.laser.set_pwr_unit('dBm')
-            self.ps.optprobe.laser.set_pwr(self.variables['pwr'])
+            self.ps.optprobe.laser.set_pwr(self.pwr)
             self.ps.optprobe.laser.set_pwr_unit('mW')
             self.ps.optprobe.laser.set_output(True)
-            time.sleep(3)
         
             self.execute()
 
-            self.ps.optprobe.laser.set_output(False)
+            self.tls.set_output(False)
 
-        
         self.ps.set_settings(settings)
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/voltage_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/voltage_sweep_ida.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,37 @@
 from dreamcreator.sequences.core.smu_sweep import SmuSweep
 
-class VoltageSweep(SmuSweep):
+class VoltageSweepIda(SmuSweep):
     """
     Voltage sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
         self.variables = {
             'Start': 0, 
             'Start_info': 'Please enter start voltage (V)',
-            'Start_bounds': [-100, 100],
             'Stop': 1, 
             'Stop_info': 'Please enter stop voltage (V)',
-            'Stop_bounds': [-100, 100],
-            'Step': 0.1, 
-            'Step_info': 'Please enter stepsize (V)',
-            'Step_bounds': [0.01, 100],
-            'Center': '',
-            'Center_info': 'Please enter center voltage',
-            'Center_bounds': [0, 100],
-            'Span': '',
-            'Span_info': 'Please enter span voltage',
-            'Span_bounds': [0, 100],
-            'Range': '',
-            'Range_info': 'Please enter range voltage',
-            'Range_bounds': [0, 100],
-            'Spacing': '',
-            'Spacing_info': 'Please enter spacing voltage',
-            'Spacing_bounds': [0, 100],
-            'Points': '',
-            'Points_info': 'Please enter points voltage',
-            'Points_bounds': [0, 1000],
-            'Direction': 'UP',
-            'Direction_info': 'Please enter direction voltage',
-            'Direction_options': ['UP', 'DOWN'],
-            'Sweeptype': 'voltage',
-            'Sweeptype_info': 'Please enter sweep type',
-            'Sweeptype_options': ['voltage'],
-            'Upper Limit': 5,
-            'Upper Limit_info': 'Please enter upper limit voltage',
-            'Upper Limit_bounds': [0, 100],
-            'Trans_col': 'False',
-            'Trans_col_info': 'Please enter transition eitehr True or False',
-            'Trans_col_options': ['True', 'False']
+            'Res': 100, 
+            'Res_info': 'Please enter stepsize (mV)',
+            'IV': 'True',
+            'IV_info': 'Enter True to receive IV plot',
+            'RV': 'True',
+            'RV_info': 'Enter True to receive RV plot',
+            'PV': 'True',
+            'PV_info': 'Enter True to receive PV plot',
+            'Channel A': 'True',
+            'Channel A_info': 'Please enter True to use Channel A if not enter False',
+            'Channel B': 'False',
+            'Channel B_info': 'Please enter True to use Channel B if not enter False'
         }
 
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
             'plottitle': 'Voltage Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Voltage (V)',
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/DREAM/wavelength_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep_ida.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,54 @@
 from dreamcreator.sequences.core.laser_sweep import LaserSweep
 
-class WavelengthSweep(LaserSweep):
+class WavelengthSweepIda(LaserSweep):
     """
     Wavelength sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
         self.variables = {
-            'Start': 1280,
+            'Start': 1480,
             'Start_info': 'unit nm',
-            'Start_bounds': [[1270, 1480], [1350, 1580]],
-            'Stop': 1370,
+            'Stop': 1580,
             'Stop_info': 'unit nm',
-            'Stop_bounds': [[1270, 1480], [1350, 1580]],
             'Step': 1,
-            'Step_info': 'unit nm, can also use wavl_pts, if both filled Step will take priority',
-            'Step_bounds': [0.01, 100],
-            'wavl_pts': 601,
-            'wavl_pts_info': 'can also use Step, if both filled Step will take priority',
-            'wavl_pts_bounds': [1, 10000],
+            'Step_info': 'unit nm',
             'Power': 1,
             'Power_info': 'unit dBm',
-            'Power_bounds': [-70, 100],
             'Sweep Speed': 'auto',
-            'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this',
-            'Sweep Speed_options': ['20nm', '10nm', 'auto'],
-            'Upper Limit': 0,
-            'Upper Limit_info': 'set to 0',
-            'Upper Limit_bounds': [-30, 0],
-            'Mode': 'CONT',
-            'Mode_info': 'choose between CONT and STEP',
-            'Mode_options': ['CONT', 'STEP'],
+            'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this, options are 20nm, 10nm, auto',
             'Laser Output': 'High Power',
-            'Laser Output_info': 'choose between High Power and Low SSE',
-            'Laser_options': ['High Power', 'Low SSE'],
+            'Laser Output_info': 'Set to High Power or Low SSE',
             'Numscans': 1,
             'Numscans_info': 'choose how many scans for each device, default 1, max 3',
-            'Numscans_bounds': [1,3],
             'RangeDec': 20,
             'RangeDec_info': 'default 20',
-            'RangeDec_bounds': [0, 100],
+            'Initialrange': '-20',
+            'Initialrange_info': 'default -20'
         }
 
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
             'plottitle': 'WavelengthSweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Wavelength (nm)',
             'ytitle': 'Power (dBm)',
             'xscale': 1,
             'yscale': 1,
             'legend': True,
             'csv': True,
             'pdf': True,
             'mat': True,
-            'pkl': True
+            'pkl': False
         }
         super().__init__(ps, variables=self.variables, resultsinfo=self.resultsinfo, mode='CONT')
         
     def run(self, routine=False):
         self.set_results(variables=self.variables, resultsinfo = self.resultsinfo, routine=routine)
         settings = self.ps.get_settings(self.verbose)
         self.execute()
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/current_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep_ida.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,39 +7,31 @@
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
         self.variables = {
             'Start': 0, 
             'Start_info': 'Please enter start current (mA)',
-            'Start_bounds': [-100, 100],
             'Stop': 1, 
             'Stop_info': 'Please enter stop current (mA)',
-            'Stop_bounds': [-100, 100],
-            'Step': 0.1, 
-            'Step_info': 'Please enter stepsize (mA)',
-            'Step_bounds': [0.01, 100],
+            'Res': 0.1, 
+            'Res_info': 'Please enter stepsize (mA)',
             'IV': 'True',
             'IV_info': 'Please enter True if you want an IV curve if not enter False',
-            'IV_options': ['True', 'False'],
             'RV': 'True',
             'RV_info': 'Please enter True if you want an RV curve if not enter False',
-            'RV_options': ['True', 'False'],
             'PV': 'True',
             'PV_info': 'Please enter True if you want a PV curve if not enter False',
-            'PV_options': ['True', 'False'],
             'Channel A': 'True',
             'Channel A_info': 'Please enter True to use Channel A if not enter False',
-            'Channel A_options': ['True', 'False'],
             'Channel B': 'False',
-            'Channel B_info': 'Please enter True to use Channel B if not enter False',
-            'Channel B_options': ['True', 'False']
+            'Channel B_info': 'Please enter True to use Channel B if not enter False'
         }
 
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
             'plottitle': 'Current Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Current (A)',
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_current_wavelength_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep_ida.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,50 +8,38 @@
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
 
         self.variables = {
             'Start': 1480,
             'Start_info': 'Please enter the start wavelength in nm',
-            'Start_bounds': [[1270, 1480], [1350, 1580]],
             'Stop': 1580,
             'Stop_info': 'Please enter the stop wavelength in nm',
-            'Stop_bounds': [[1270, 1480], [1350, 1580]],
             'Step': 1,
             'Step_info': 'Please enter the step size in nm',
-            'Step_bounds': [0.01, 10],
             'Power': 1,
             'Power_info': 'Please enter the power in dBm',
-            'Power_bounds': [-70, 10],
             'Sweep Speed': 'auto',
             'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this, options are 20nm, 10nm, auto',
-            'Sweep Speed_options': ['20nm', '10nm', 'auto'],
             'Laser Output': 'High Power',
             'Laser Output_info': 'Set to High Power or Low SSE',
-            'Laser Output_options': ['High Power', 'Low SSE'],
             'Numscans': 1,
             'Numscans_info': 'choose how many scans for each device, default 1, max 3',
-            'Numscans_bounds': [1,3],
             'RangeDec': 20,
             'RangeDec_info': 'default 20',
-            'RangeDec_bounds': [0, 100],
             'Initialrange': '-20',
             'Initialrange_info': 'default -20',
-            'Initialrange_bounds': [-100, 100],
             'Channel A': 'True',
             'Channel A_info': 'Please enter True to use Channel A if not enter False',
-            'Channel A_options': ['True','False'],
             'Channel B': 'False',
             'Channel B_info': 'Please enter True to use Channel B if not enter False',
-            'Channel B_options': ['True','False'],
             'Currents': '0, 1, 2',
-            'Currents_info': 'Please format the currents in units (A) as a list of integers separated by commas ex. 0, 1, 2',
-            'Currents_bounds': [-100, 100],
+            'Currents_info': 'Please format the currents in units (A) as a list of integers separated by commas ex. 0, 1, 2'
         }
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
             'plottitle': 'Set Current Wavelength Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Wavelength (nm)',
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,40 @@
 from dreamcreator.sequences.core.laser_sweep import LaserSweep
 
-class SetVoltageWavelengthSweepIda(LaserSweep):
+class SetVoltageWavelengthSweep(LaserSweep):
     """
     Sets the voltage and then performs a laser sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
 
         self.variables = {
             'Start': 1480,
-            'Start_info': 'unit nm',
-            'Start_bounds': [[1270, 1480], [1350, 1580]],   
+            'Start_info': 'Please enter a value for the start wavelength in nm',
             'Stop': 1580,
-            'Stop_info': 'unit nm',
-            'Stop_bounds': [[1270, 1480], [1350, 1580]],
+            'Stop_info': 'Please enter a value for the stop wavelength in nm',
             'Step': 1,
-            'Step_info': 'unit nm, can also use wavl_pts, if both filled Step will take priority',
-            'Step_bounds': [0.01, 10],
+            'Step_info': 'Please enter a value for the step size in nm',
+            'wavl_pts': 101,
+            'wavl_pts_info': 'Please enter a value for the number of points in the wavelength sweep',
             'Power': 1,
-            'Power_info': 'unit dBm',
-            'Power_bounds': [-70, 10],
-            'Sweep Speed': 'auto',
-            'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this, options are 20nm, 10nm, auto',
-            'Sweep Speed_options': ['20nm', '10nm', 'auto'],
-            'Laser Output': 'High Power',
-            'Laser Output_info': 'Set to High Power or Low SSE',
-            'Laser Output_options': ['High Power', 'Low SSE'],
-            'Numscans': 1,
-            'Numscans_info': 'choose how many scans for each device, default 1, max 3',
-            'Numscans_bounds': [1,3],
-            'RangeDec': 20,
-            'RangeDec_info': 'default 20',
-            'RangeDec_bounds': [0, 100],
-            'Initialrange': '-20',
-            'Initialrange_info': 'default -20',
-            'Initialrange_bounds': [-100, 100],
-            'Channel A': 'True',
-            'Channel A_info': 'Please enter True to use Channel A if not enter False',
-            'Channel A_options': ['True','False'],
-            'Channel B': 'False',
-            'Channel B_info': 'Please enter True to use Channel B if not enter False',
-            'Channel B_options': ['True','False'],
-            'Voltages': '0, 1, 2',
-            'Voltages_info': 'Please enter voltages in units (V) in the form x1, x2, x3',
-            'Voltages_bounds': [-50, 50]
+            'Power_info': 'Please enter a value for the power in dBm',
+            'Sweep Speed': 20,
+            'Sweep Speed_info': 'Please enter a value for the sweep speed in nm/s',
+            'Upper Limit': 0,
+            'Upper Limit_info': 'Please enter a value for the upper limit of the sweep in dBm',
+            'Mode': 'CONT',
+            'Mode_info': 'Please select a mode from the following options: CONT, STEP, RAMP, SINE, SQUARE, TRIANGLE',
+            'Voltages': '[0, 1, 2]',
+            'Voltages_info': 'Please format the voltages as a list of integers separated by commas ex. [0,1,2]'
         }
-        self.results_info = {
+
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
             'plottitle': 'Set Voltage Wavelength Sweep',
             'save_location': '',
             'foldername': '',
             'xtitle': 'Wavelength (nm)',
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_wavelength_current_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_voltage_sweep_ida.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,71 @@
 from dreamcreator.sequences.core.smu_sweep import SmuSweep
+import time
 
-class SetWavelengthCurrentSweepIda(SmuSweep):
+class SetWavelengthVoltageSweepIda(SmuSweep):
     """
-    Sets the wavelength then performs a current sweep.
+    Sets the wavelength then performs a voltage sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
-
         self.variables = {
             'Start': 0, 
-            'Start_info': 'Please enter start current (mA)',
-            'Start_bounds': [-1000, 1000],
+            'Start_info': 'Please enter start voltage (V)',
             'Stop': 1, 
-            'Stop_info': 'Please enter stop current (mA)',
-            'Stop_bounds': [-1000, 1000],
-            'Step': 0.1, 
-            'Step_info': 'Please enter step current (mA)',
-            'Step_bounds': [0.01, 1000],
+            'Stop_info': 'Please enter stop voltage (V)',
+            'Res': 100, 
+            'Res_info': 'Please enter step voltage (mV)',
             'IV': 'True',
             'IV_info': 'True if current vs voltage plot needed',
-            'IV_options': ['True', 'False'],
             'RV': 'True',
-            'RV_info': 'True if resistance vs voltage plot needed',
-            'RV_options': ['True', 'False'],
+            'RV_info': 'True if ressiatnce vs voltage plot needed',
             'PV': 'True',
             'PV_info': 'True if power vs voltage plot needed',
-            'PV_options': ['True', 'False'],
             'Channel A': 'True',
             'Channel A_info': 'Please enter True to use Channel A if not enter False',
-            'Channel A_options': ['True', 'False'],
             'Channel B': 'False',
             'Channel B_info': 'Please enter True to use Channel B if not enter False',
-            'Channel B_options': ['True', 'False'],
             'Wavelengths': '1480, 1550, 1580',
-            'Wavelengths_info': 'Set wavelengths in form x, x1, x2 with unit nm',
-            'Wavelengths_bounds': [[1270, 1480], [1350, 1580]]
+            'Wavelengths_info': 'Set wavelengths in form x, x1, x2 with unit nm'
         }
 
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
-            'plottitle': 'Set Wavelength Current Sweep',
+            'plottitle': 'Set Wavelength Voltage Sweep',
             'save_location': '',
             'foldername': '',
-            'xtitle': 'Current (A)',
-            'ytitle': 'Voltage (V)',
+            'xtitle': 'Voltage (V)',
+            'ytitle': 'Current (A)',
             'xscale': 1,
             'yscale': 1,
             'legend': True,
             'csv': True,
             'pdf': True,
             'mat': True,
             'pkl': False
         }
 
-        super().__init__(variable=self.variables, resultsinfo=self.resultsinfo, type='current', ps=ps)
+        super().__init__(variables=self.variables, resultsinfo=self.resultsinfo, sweeptype='voltage', ps=ps)
 
     def run(self, routine=False):
         self.set_results(variables=self.variables, resultsinfo = self.resultsinfo, routine=routine)
 
         settings = self.ps.get_settings(self.verbose)
 
-        for wav in self.wavelengths:
+        for wav in self.variables['wavelengths']:
             self.ps.optprobe.laser.set_wavl(wav)
             self.ps.optprobe.laser.set_pwr_unit('dBm')
-            self.ps.optprobe.laser.set_pwr(self.pwr)
+            self.ps.optprobe.laser.set_pwr(self.variables['pwr'])
             self.ps.optprobe.laser.set_pwr_unit('mW')
             self.ps.optprobe.laser.set_output(True)
+            time.sleep(3)
         
             self.execute()
 
-            self.tls.set_output(False)
+            self.ps.optprobe.laser.set_output(False)
 
+        
         self.ps.set_settings(settings)
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,64 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
-import time
+from dreamcreator.sequences.core.laser_sweep import LaserSweep
 
-class SetWavelengthVoltageSweepIda(SmuSweep):
+class WavelengthSweep(LaserSweep):
     """
-    Sets the wavelength then performs a voltage sweep.
+    Wavelength sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
     """
     def __init__(self, ps):
         self.variables = {
-            'Start': 0, 
-            'Start_info': 'Please enter start voltage (V)',
-            'Start_bounds': [-100, 100],
-            'Stop': 1, 
-            'Stop_info': 'Please enter stop voltage (V)',
-            'Stop_bounds': [-100, 100],
-            'Step': 0.1, 
-            'Step_info': 'Please enter step voltage (V)',
-            'Step_bounds': [0.01, 100],
-            'IV': 'True',
-            'IV_info': 'True if current vs voltage plot needed',
-            'IV_options': ['True', 'False'],
-            'RV': 'True',
-            'RV_info': 'True if ressiatnce vs voltage plot needed',
-            'RV_options': ['True', 'False'],
-            'PV': 'True',
-            'PV_info': 'True if power vs voltage plot needed',
-            'PV_options': ['True', 'False'],
-            'Channel A': 'True',
-            'Channel A_info': 'Please enter True to use Channel A if not enter False',
-            'Channel A_options': ['True', 'False'],
-            'Channel B': 'False',
-            'Channel B_info': 'Please enter True to use Channel B if not enter False',
-            'Channel B_options': ['True', 'False'],
-            'Wavelengths': '1480, 1550, 1580',
-            'Wavelengths_info': 'Set wavelengths in form x, x1, x2 with unit nm',
-            'Wavelengths_bounds': [[1270, 1480], [1350, 1580]]
+            'Start': 1280,
+            'Start_info': 'unit nm',
+            'Stop': 1370,
+            'Stop_info': 'unit nm',
+            'Step': 1,
+            'Step_info': 'unit nm, can also use wavl_pts, if both filled Step will take priority',
+            'wavl_pts': 601,
+            'wavl_pts_info': 'can also use Step, if both filled Step will take priority',
+            'Power': 1,
+            'Power_info': 'unit dBm',
+            'Sweep Speed': 20,
+            'Sweep Speed_info': 'controls the speed of the sweep, if yaml fails time execution test increase this',
+            'Upper Limit': 0,
+            'Upper Limit_info': 'set to 0',
+            'Mode': 'CONT',
+            'Mode_info': 'choose between CONT and STEP',
+            'Laser Output': 'High Power',
+            'Laser Output_info': 'choose between CONT and STEP',
+            'Numscans': 1,
+            'Numscans_info': 'choose between CONT and STEP',
+            'RangeDec': '20',
+            'RangeDec_info': 'choose between CONT and STEP'
+        
         }
 
-        self.results_info = {
+        self.resultsinfo = {
             'num_plots': 1,
             'visual': True,
             'saveplot': True,
-            'plottitle': 'Set Wavelength Voltage Sweep',
+            'plottitle': 'WavelengthSweep',
             'save_location': '',
             'foldername': '',
-            'xtitle': 'Voltage (V)',
-            'ytitle': 'Current (A)',
+            'xtitle': 'Wavelength (nm)',
+            'ytitle': 'Power (dBm)',
             'xscale': 1,
             'yscale': 1,
             'legend': True,
             'csv': True,
             'pdf': True,
             'mat': True,
-            'pkl': False
+            'pkl': True
         }
-
-        super().__init__(variables=self.variables, resultsinfo=self.resultsinfo, sweeptype='voltage', ps=ps)
-
+        super().__init__(ps, variables=self.variables, resultsinfo=self.resultsinfo, mode='CONT')
+        
     def run(self, routine=False):
         self.set_results(variables=self.variables, resultsinfo = self.resultsinfo, routine=routine)
-
         settings = self.ps.get_settings(self.verbose)
+        self.execute()
 
-        for wav in self.variables['wavelengths']:
-            self.ps.optprobe.laser.set_wavl(wav)
-            self.ps.optprobe.laser.set_pwr_unit('dBm')
-            self.ps.optprobe.laser.set_pwr(self.variables['pwr'])
-            self.ps.optprobe.laser.set_pwr_unit('mW')
-            self.ps.optprobe.laser.set_output(True)
-            time.sleep(3)
-        
-            self.execute()
+        self.ps.set_settings(settings)
 
-            self.ps.optprobe.laser.set_output(False)
 
-        
-        self.ps.set_settings(settings)
+
```

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/core/laser_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/laser_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/core/results.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/results.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/core/sequence.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/sequence.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/core/smu_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/smu_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequences/template/__init__.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/template/__init__.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.24/app/dreamcreator/sequencetracker.py` & `DreamCreator-0.0.3/app/dreamcreator/sequencetracker.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.24/app/dreamcreator/yamlcheck.py` & `DreamCreator-0.0.3/app/dreamcreator/yamlcheck.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import yaml
 
-
 def get_key_at_position(some_dict, position=1):
     """
     Retrieves the key at a specified position from a dictionary.
 
     Args:
     some_dict (dict): The dictionary from which to retrieve the key.
     position (int): Position of the key to retrieve, 1-based indexing. Default is 1.
@@ -12,146 +11,105 @@
     Returns:
     The key at the specified position, or None if the position is out of range.
     """
     if 1 <= position <= len(some_dict):
         return list(some_dict)[position - 1]
     return None
 
-
 def yaml_check(yaml_file_path):
     """
     Reads a YAML file and converts it to a dictionary.
 
     Args:
     yaml_file_path (str): Path to the YAML file.
 
     Returns:
     dict: Dictionary representation of the YAML file.
     """
-    errorflag = False
-    with open(yaml_file_path, "r") as file:
+    errorflag = False 
+    with open(yaml_file_path, 'r') as file:
         try:
             yaml_dict = yaml.safe_load(file)
         except yaml.YAMLError as exc:
             print(exc)
             errorflag = True
-            print("Error in YAML file. Please check the file and try again.")
+            print('Error in YAML file. Please check the file and try again.')
             return None
-
-    try:
+        
+    
+    try:    
         deviceflag = get_key_at_position(yaml_dict, 1)
         sequenceflag = get_key_at_position(yaml_dict, 2)
     except:
         errorflag = True
-        print("Error in YAML file. Please check the file and try again.")
+        print('Error in YAML file. Please check the file and try again.')
         return None
+    
 
-    if deviceflag != "Devices":
+    if deviceflag != 'Devices':
         errorflag = True
-        print("Error in YAML file. Please check the file and try again.")
+        print('Error in YAML file. Please check the file and try again.')
         return None
-
-    if sequenceflag != "Sequences":
+    
+    if sequenceflag != 'Sequences':
         errorflag = True
-        print("Error in YAML file. Please check the file and try again.")
+        print('Error in YAML file. Please check the file and try again.')
         return None
+    
+    # 
 
-    #
-
-    # check for sequence runtime errors
+    #check for sequence runtime errors
     runtime = sequence_runtime_check(yaml_dict, True)
-    print("Sequence runtime: ", runtime)
-
-
+    print('Sequence runtime: ', runtime)
+    
 def sequence_runtime_check(yaml_file_path, dict=None):
     """
     Checks the runtime of a sequence.
     """
     if dict == None:
-        with open(yaml_file_path, "r") as file:
+        with open(yaml_file_path, 'r') as file:
             try:
                 yaml_dict = yaml.safe_load(file)
             except yaml.YAMLError as exc:
                 print(exc)
                 errorflag = True
-                print("Error in YAML file. Please check the file and try again.")
+                print('Error in YAML file. Please check the file and try again.')
                 return None
     else:
         yaml_dict = yaml_file_path
-
-    sequences = yaml_dict["Sequences"]
-    # calculate wavlength sweep runtime
+        
+    sequences = yaml_dict['Sequences']
+    #calculate wavlength sweep runtime
 
     wavelength_constant = 10
     smu_constant = 10
 
-    sequencetypes = [
-        "wavelength_sweep",
-        "current_sweep",
-        "voltage_sweep",
-        "set_current_wavelength_sweep",
-        "set_voltage_wavelength_sweep",
-        "set_wavelength_current_sweep",
-        "set_wavelength_voltage_sweep",
-    ]
+    sequencetypes = ['wavelength_sweep', 'current_sweep', 'voltage_sweep', 'set_current_wavelength_sweep', 'set_voltage_wavelength_sweep', 'set_wavelength_current_sweep', 'set_wavelength_voltage_sweep']
 
-    for sequence in sequences:
+    for sequence in sequences: 
 
         seq = sequences[sequence]
-        variables = seq["variables"]
-        # print(variables)
+        variables = seq['variables']
+        #print(variables)
         if sequencetypes[6] in sequence:
-            runtime = (
-                (
-                    (float(variables["stop"]) - float(variables["start"]))
-                    / float(variables["step"])
-                )
-                * smu_constant
-                * (variables["wavelengths"].count(",") + 1)
-            )
+            runtime = ((float(variables['stop']) - float(variables['start']))/float(variables['step']))*smu_constant*(variables['wavelengths'].count(',') + 1)
         elif sequencetypes[5] in sequence:
-            runtime = (
-                (
-                    (float(variables["stop"]) - float(variables["start"]))
-                    / float(variables["step"])
-                )
-                * smu_constant
-                * (variables["wavelengths"].count(",") + 1)
-            )
+            runtime = ((float(variables['stop']) - float(variables['start']))/float(variables['step']))*smu_constant*(variables['wavelengths'].count(',') + 1)
         elif sequencetypes[4] in sequence:
-            runtime = (
-                float(variables["sweep_speed"])
-                * float(variables["wavl_pts"])
-                * wavelength_constant
-                * (variables["voltages"].count(",") + 1)
-            )
+            runtime = float(variables['sweep_speed'])*float(variables['wavl_pts'])*wavelength_constant*(variables['voltages'].count(',') + 1)
         elif sequencetypes[3] in sequence:
-            runtime = (
-                float(variables["sweep_speed"])
-                * float(variables["wavl_pts"])
-                * wavelength_constant
-                * (variables["currents"].count(",") + 1)
-            )
+            runtime = float(variables['sweep_speed'])*float(variables['wavl_pts'])*wavelength_constant*(variables['currents'].count(',') + 1)
         elif sequencetypes[2] in sequence:
-            runtime = (
-                (float(variables["stop"]) - float(variables["start"]))
-                / float(variables["step"])
-            ) * smu_constant
+            runtime = ((float(variables['stop']) - float(variables['start']))/float(variables['step']))*smu_constant
         elif sequencetypes[1] in sequence:
-            runtime = (
-                (float(variables["stop"]) - float(variables["start"]))
-                / float(variables["step"])
-            ) * smu_constant
+            runtime = ((float(variables['stop']) - float(variables['start']))/float(variables['step']))*smu_constant
         elif sequencetypes[0] in sequence:
-            runtime = (
-                float(variables["sweep_speed"])
-                * float(variables["wavl_pts"])
-                * wavelength_constant
-            )
+            runtime = float(variables['sweep_speed'])*float(variables['wavl_pts'])*wavelength_constant
         else:
-            print("Error in YAML file sequences portion")
+            print('Error in YAML file sequences portion')
             return None
         return runtime
 
+    
 
 # Example usage
-# yaml_dict = yaml_check(r'D:\Work\Github_repo\DreamLab\Examples\test.yaml')
+#yaml_dict = yaml_check(r'D:\Work\Github_repo\DreamLab\Examples\test.yaml')
```

### Comparing `DreamCreator-0.0.24/setup.py` & `DreamCreator-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "DreamCreator",
-    version = "0.0.24",
+    version = "0.0.3",
     description = "A tool for creating YAML files for use in Dream Photonics and edx course",
     package_dir = {"": "app"},
     packages = find_packages(where="app"),
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/dreamphotonics/DreamCreator.git",
     author = "Jonathan Barnes",
     author_email = "jonathanyorkbarnes@gmail.com",
     license="MIT",
     classifiers=[
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[    
-        'numpy>=1.26.3',
-        'pandas>=2.2.0',
-        'pillow>=10.2.0',
+        'numpy==1.26.3',
+        'pandas==2.2.0',
+        'pillow==10.2.0',
         'pkginfo==1.10.0',
         'PyQt5>=5.15.10',
         'PyQt5-Qt5>=5.15.2',
-        'PyQt5-sip>=12.13.0',
-        'pywin32-ctypes>=0.2.2',
-        'PyYAML>=6.0.1',
-        'scipy>=1.12.0',
-        'twine>=5.0.0',
-        'watchdog>=3.0.0',
-        'matplotlib>=3.8.2'
+        'PyQt5-sip==12.13.0',
+        'pywin32-ctypes==0.2.2',
+        'PyYAML==6.0.1',
+        'scipy==1.12.0',
+        'twine==5.0.0',
+        'watchdog==3.0.0',
+        'matplotlib==3.8.2'
     ],
-    python_requires='>=3.10',
+    python_requires='>=3.11',
 )
```

