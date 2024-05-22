# Comparing `tmp/notebooks_and_scripts-4.451.1.tar.gz` & `tmp/notebooks_and_scripts-4.452.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooks_and_scripts-4.451.1.tar", last modified: Tue May 21 02:41:17 2024, max compression
+gzip compressed data, was "notebooks_and_scripts-4.452.1.tar", last modified: Tue May 21 04:16:06 2024, max compression
```

## Comparing `notebooks_and_scripts-4.451.1.tar` & `notebooks_and_scripts-4.452.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:41:17.651579 notebooks_and_scripts-4.451.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.451.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:51:23.000000 notebooks_and_scripts-4.451.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     5625 2024-05-21 02:41:17.650838 notebooks_and_scripts-4.451.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.451.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:41:17.646870 notebooks_and_scripts-4.451.1/notebooks_and_scripts/
--rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-21 02:41:12.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      259 2024-05-20 22:32:21.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:41:17.649443 notebooks_and_scripts-4.451.1/notebooks_and_scripts/sagemaker/
--rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts/sagemaker/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:41:17.650040 notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     5625 2024-05-21 02:41:17.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      515 2024-05-21 02:41:17.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 02:41:17.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      164 2024-05-21 02:41:17.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-21 02:41:17.000000 notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      366 2024-05-20 22:39:52.000000 notebooks_and_scripts-4.451.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 02:41:17.651851 notebooks_and_scripts-4.451.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)     1076 2024-05-20 04:52:45.000000 notebooks_and_scripts-4.451.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 04:16:06.925012 notebooks_and_scripts-4.452.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.452.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:51:23.000000 notebooks_and_scripts-4.452.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-05-21 04:16:06.924526 notebooks_and_scripts-4.452.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.452.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 04:16:06.918889 notebooks_and_scripts-4.452.1/notebooks_and_scripts/
+-rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-21 04:16:00.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      259 2024-05-20 22:32:21.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 04:16:06.922895 notebooks_and_scripts-4.452.1/notebooks_and_scripts/sagemaker/
+-rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts/sagemaker/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 04:16:06.923798 notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-05-21 04:16:06.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      530 2024-05-21 04:16:06.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 04:16:06.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      164 2024-05-21 04:16:06.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-21 04:16:06.000000 notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 04:14:57.000000 notebooks_and_scripts-4.452.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      366 2024-05-20 22:39:52.000000 notebooks_and_scripts-4.452.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 04:16:06.925108 notebooks_and_scripts-4.452.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      352 2024-05-21 04:15:39.000000 notebooks_and_scripts-4.452.1/setup.py
```

### Comparing `notebooks_and_scripts-4.451.1/LICENSE` & `notebooks_and_scripts-4.452.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.451.1/PKG-INFO` & `notebooks_and_scripts-4.452.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.451.1
+Version: 4.452.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Home-page: https://github.com/kamangir/notebooks-and-scripts
-Author: arash@kamangir.net
+Author: Arash Abadpour (Kamangir)
+Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,28 +28,28 @@
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 # 📜 notebooks & [meta] scripts
 
-[notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for ai experiments and aws batch jobs.
+[notebooks](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks) and [scripts](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts) for ai experiments and aws batch jobs.
 
 ---
 
 | ![image](https://github.com/kamangir/assets/blob/main/nbs/3x4.jpg?raw=true)                               | ![image](https://github.com/kamangir/assets/blob/main/nbs/mission-patch-00008.png?raw=true) | ![image](https://github.com/kamangir/assets/blob/main/nbs/train-summary.png?raw=true) ![image](https://github.com/kamangir/assets/blob/main/nbs/predict-00000.png?raw=true) |
 | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/roofAI-train.sh)                                                                                                                                   |
+| [paint-a-sentence](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/roofAI-train.sh)                                                                                                                                   |
 | https://medium.com/@arash-kamangir/a-cat-walking-under-apple-trees-style-by-stable-diffusion-ab60ece43e2a | https://medium.com/@arash-kamangir/private-mission-patch-%EF%B8%8F-1-0c2eddd79762           | https://arash-kamangir.medium.com/roofai-%EF%B8%8F-on-gpu-6-b02f8f67ed3f                                                                                                    |
 
-also: [`sagesemseg`](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/sagesemseg/).
+also: [`sagesemseg`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/sagesemseg/).
 
 ---
 
-also home to [`workflow`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
+also home to [`workflow`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
 
 ```bash
  > workflow help
 workflow create \
 	pattern=a-bc-d|hourglass,~upload \
 	-|<job-name> \
 	<command-line>
@@ -68,14 +69,14 @@
 workflow create pattern=hourglass .
 workflow submit to=aws_batch
 @watch - @download
 ```
 
 from https://arash-kamangir.medium.com/%EF%B8%8F-openai-experiments-54-e49117dc69ef
 
-| [`a-bc-d`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
+| [`a-bc-d`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
 | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true)                                                              | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true)                                                                    | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true)                                                                      |
 
 ---
 
 To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `nbs` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `notebooks_and_scripts-4.451.1/README.md` & `notebooks_and_scripts-4.452.1/README.md`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/PKG-INFO` & `notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.451.1
+Version: 4.452.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Home-page: https://github.com/kamangir/notebooks-and-scripts
-Author: arash@kamangir.net
+Author: Arash Abadpour (Kamangir)
+Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,28 +28,28 @@
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 # 📜 notebooks & [meta] scripts
 
-[notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for ai experiments and aws batch jobs.
+[notebooks](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks) and [scripts](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts) for ai experiments and aws batch jobs.
 
 ---
 
 | ![image](https://github.com/kamangir/assets/blob/main/nbs/3x4.jpg?raw=true)                               | ![image](https://github.com/kamangir/assets/blob/main/nbs/mission-patch-00008.png?raw=true) | ![image](https://github.com/kamangir/assets/blob/main/nbs/train-summary.png?raw=true) ![image](https://github.com/kamangir/assets/blob/main/nbs/predict-00000.png?raw=true) |
 | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/roofAI-train.sh)                                                                                                                                   |
+| [paint-a-sentence](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/roofAI-train.sh)                                                                                                                                   |
 | https://medium.com/@arash-kamangir/a-cat-walking-under-apple-trees-style-by-stable-diffusion-ab60ece43e2a | https://medium.com/@arash-kamangir/private-mission-patch-%EF%B8%8F-1-0c2eddd79762           | https://arash-kamangir.medium.com/roofai-%EF%B8%8F-on-gpu-6-b02f8f67ed3f                                                                                                    |
 
-also: [`sagesemseg`](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/sagesemseg/).
+also: [`sagesemseg`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/scripts/sagesemseg/).
 
 ---
 
-also home to [`workflow`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
+also home to [`workflow`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
 
 ```bash
  > workflow help
 workflow create \
 	pattern=a-bc-d|hourglass,~upload \
 	-|<job-name> \
 	<command-line>
@@ -68,14 +69,14 @@
 workflow create pattern=hourglass .
 workflow submit to=aws_batch
 @watch - @download
 ```
 
 from https://arash-kamangir.medium.com/%EF%B8%8F-openai-experiments-54-e49117dc69ef
 
-| [`a-bc-d`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
+| [`a-bc-d`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://raw.githubusercontent.com/kamangir/notebooks-and-scripts/main/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
 | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true)                                                              | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true)                                                                    | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true)                                                                      |
 
 ---
 
 To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `nbs` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `notebooks_and_scripts-4.451.1/notebooks_and_scripts.egg-info/SOURCES.txt` & `notebooks_and_scripts-4.452.1/notebooks_and_scripts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 notebooks_and_scripts/__init__.py
 notebooks_and_scripts/__main__.py
 notebooks_and_scripts/config.env
 notebooks_and_scripts/env.py
 notebooks_and_scripts/logger.py
```

