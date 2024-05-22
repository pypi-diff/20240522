# Comparing `tmp/kamangir-3.38.1.tar.gz` & `tmp/kamangir-3.40.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kamangir-3.38.1.tar", last modified: Mon May 20 01:29:34 2024, max compression
+gzip compressed data, was "kamangir-3.40.1.tar", last modified: Tue May 21 02:53:18 2024, max compression
```

## Comparing `kamangir-3.38.1.tar` & `kamangir-3.40.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 01:29:34.875980 kamangir-3.38.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.38.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)     3431 2024-05-20 01:29:34.875337 kamangir-3.38.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3266 2024-04-22 03:51:11.000000 kamangir-3.38.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 01:29:34.872967 kamangir-3.38.1/kamangir/
--rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-20 01:29:31.000000 kamangir-3.38.1/kamangir/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-03-04 08:06:58.000000 kamangir-3.38.1/kamangir/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4622 2024-03-26 02:01:13.000000 kamangir-3.38.1/kamangir/content.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-03-04 08:06:21.000000 kamangir-3.38.1/kamangir/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:48.000000 kamangir-3.38.1/kamangir/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-12 02:59:04.000000 kamangir-3.38.1/kamangir/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-20 01:29:34.874766 kamangir-3.38.1/kamangir.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     3431 2024-05-20 01:29:34.000000 kamangir-3.38.1/kamangir.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      274 2024-05-20 01:29:34.000000 kamangir-3.38.1/kamangir.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-20 01:29:34.000000 kamangir-3.38.1/kamangir.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-20 01:29:34.000000 kamangir-3.38.1/kamangir.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-20 01:29:34.876120 kamangir-3.38.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      488 2024-05-20 01:29:24.000000 kamangir-3.38.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:53:18.876500 kamangir-3.40.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.40.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:43.000000 kamangir-3.40.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-21 02:53:18.875905 kamangir-3.40.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3243 2024-05-21 02:52:53.000000 kamangir-3.40.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:53:18.873636 kamangir-3.40.1/kamangir/
+-rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-21 02:53:15.000000 kamangir-3.40.1/kamangir/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4623 2024-05-21 02:51:34.000000 kamangir-3.40.1/kamangir/content.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-21 02:51:14.000000 kamangir-3.40.1/kamangir/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:53:18.875432 kamangir-3.40.1/kamangir.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      303 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-21 02:53:18.000000 kamangir-3.40.1/kamangir.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      475 2024-05-20 22:39:45.000000 kamangir-3.40.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 02:53:18.876599 kamangir-3.40.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      488 2024-05-20 01:29:24.000000 kamangir-3.40.1/setup.py
```

### Comparing `kamangir-3.38.1/LICENSE` & `kamangir-3.40.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kamangir-3.38.1/PKG-INFO` & `kamangir-3.40.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: kamangir
-Version: 3.38.1
+Version: 3.40.1
 Summary: kamangir.net
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 My name is [Arash](http://kamangir.net/); I mix [ai](https://github.com/kamangir/roofAI), [cloud](https://github.com/kamangir/hubble), and [mathematics](https://github.com/kamangir/giza) into minimal forms that seek survival.
 
 
-| [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks for experiments & [meta] scripts for aws batch jobs and sagemaker serving. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 A recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
+| [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks and scripts for ai experiments and aws batch jobs. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 a recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
 | --- | --- | --- | --- |
 | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/carrot.png)](https://github.com/kamangir/openai_cli) 🛠️ tools for the OpenAI API | [![image](https://github.com/kamangir/hubble/raw/main/assets/hst/u4ge0106r_c0m.gif)](https://github.com/kamangir/hubble) 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry. | [![image](https://github.com/kamangir/AI-ART/raw/main/blue-stability/blue_stability.gif)](https://github.com/kamangir/blue-stability) bash cli for stability.ai API's stable diffusion inference | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/DALL-E.png?raw=1)](https://github.com/kamangir/aiart) tools for AiArt. |
 | [![image](https://github.com/kamangir/awesome-bash-cli/raw/main/assets/marquee.png)](https://github.com/kamangir/awesome-bash-cli) 🚀 a language to speak AI. | [![image](https://user-images.githubusercontent.com/1007567/221448494-d57e08c1-625b-499e-a576-81894f112d6a.jpg)](https://github.com/kamangir/ferfereh) 3d-printed graffiti | [![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/Canadians_v11.gif)](https://github.com/kamangir/Kanata) a multi-screen video feed that is comprised of a matrix of animated faces that slide to the right. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/dec82-6.jpg)](https://github.com/kamangir/dec82) A wearable Raspberry Pi + Grove / Qwiic + Camera. |
 | [![image](https://github.com/kamangir/blue-rvr/raw/master/abcli/assets/marquee.jpeg)](https://github.com/kamangir/blue-rvr) a bash cli for Sphero RVR SDK - runs deep learning vision models on a Raspberry Pi using Python and TensorFlow. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/marquee.jpg)](https://github.com/kamangir/blue-bracket) a parametric 3d-printed bracket to build hardware for machine vision & ai on raspberry pi and jetson nano on the edge. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/blue3-1.jpg)](https://github.com/kamangir/blue-sbc) python + bash bootstrap for edge computing on single board computers. |  |
 
 ---
-built by [`abcli-8.82.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.31.1`](https://github.com/kamangir/kamangir).
+built by [`abcli-8.202.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.38.1`](https://github.com/kamangir/kamangir).
```

### Comparing `kamangir-3.38.1/README.md` & `kamangir-3.40.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 My name is [Arash](http://kamangir.net/); I mix [ai](https://github.com/kamangir/roofAI), [cloud](https://github.com/kamangir/hubble), and [mathematics](https://github.com/kamangir/giza) into minimal forms that seek survival.
 
 
-| [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks for experiments & [meta] scripts for aws batch jobs and sagemaker serving. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 A recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
+| [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks and scripts for ai experiments and aws batch jobs. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 a recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
 | --- | --- | --- | --- |
 | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/carrot.png)](https://github.com/kamangir/openai_cli) 🛠️ tools for the OpenAI API | [![image](https://github.com/kamangir/hubble/raw/main/assets/hst/u4ge0106r_c0m.gif)](https://github.com/kamangir/hubble) 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry. | [![image](https://github.com/kamangir/AI-ART/raw/main/blue-stability/blue_stability.gif)](https://github.com/kamangir/blue-stability) bash cli for stability.ai API's stable diffusion inference | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/DALL-E.png?raw=1)](https://github.com/kamangir/aiart) tools for AiArt. |
 | [![image](https://github.com/kamangir/awesome-bash-cli/raw/main/assets/marquee.png)](https://github.com/kamangir/awesome-bash-cli) 🚀 a language to speak AI. | [![image](https://user-images.githubusercontent.com/1007567/221448494-d57e08c1-625b-499e-a576-81894f112d6a.jpg)](https://github.com/kamangir/ferfereh) 3d-printed graffiti | [![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/Canadians_v11.gif)](https://github.com/kamangir/Kanata) a multi-screen video feed that is comprised of a matrix of animated faces that slide to the right. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/dec82-6.jpg)](https://github.com/kamangir/dec82) A wearable Raspberry Pi + Grove / Qwiic + Camera. |
 | [![image](https://github.com/kamangir/blue-rvr/raw/master/abcli/assets/marquee.jpeg)](https://github.com/kamangir/blue-rvr) a bash cli for Sphero RVR SDK - runs deep learning vision models on a Raspberry Pi using Python and TensorFlow. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/marquee.jpg)](https://github.com/kamangir/blue-bracket) a parametric 3d-printed bracket to build hardware for machine vision & ai on raspberry pi and jetson nano on the edge. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/blue3-1.jpg)](https://github.com/kamangir/blue-sbc) python + bash bootstrap for edge computing on single board computers. |  |
 
 ---
-built by [`abcli-8.82.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.31.1`](https://github.com/kamangir/kamangir).
+built by [`abcli-8.202.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.38.1`](https://github.com/kamangir/kamangir).
```

### Comparing `kamangir-3.38.1/kamangir/__main__.py` & `kamangir-3.40.1/kamangir/__main__.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.38.1/kamangir/content.py` & `kamangir-3.40.1/kamangir/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abcli import DESCRIPTION as abcli_DESCRIPTION
 from hubble import DESCRIPTION as hubble_DESCRIPTION
-from giza import DESCRIPTION as giza_DESCRIPTION
+from gizai import DESCRIPTION as giza_DESCRIPTION
 from openai_cli import DESCRIPTION as openai_cli_DESCRIPTION
 from notebooks_and_scripts import DESCRIPTION as nbs_DESCRIPTION
 from roofAI import DESCRIPTION as roofAI_DESCRIPTION
 from vancouver_watching import DESCRIPTION as vancouver_watching_DESCRIPTION
 
 content = {
     "cols": 4,
```

### Comparing `kamangir-3.38.1/kamangir/functions.py` & `kamangir-3.40.1/kamangir/functions.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.38.1/kamangir.egg-info/PKG-INFO` & `kamangir-3.40.1/kamangir.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: kamangir
-Version: 3.38.1
+Version: 3.40.1
 Summary: kamangir.net
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 My name is [Arash](http://kamangir.net/); I mix [ai](https://github.com/kamangir/roofAI), [cloud](https://github.com/kamangir/hubble), and [mathematics](https://github.com/kamangir/giza) into minimal forms that seek survival.
 
 
-| [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks for experiments & [meta] scripts for aws batch jobs and sagemaker serving. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 A recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
+| [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks and scripts for ai experiments and aws batch jobs. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 a recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
 | --- | --- | --- | --- |
 | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/carrot.png)](https://github.com/kamangir/openai_cli) 🛠️ tools for the OpenAI API | [![image](https://github.com/kamangir/hubble/raw/main/assets/hst/u4ge0106r_c0m.gif)](https://github.com/kamangir/hubble) 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry. | [![image](https://github.com/kamangir/AI-ART/raw/main/blue-stability/blue_stability.gif)](https://github.com/kamangir/blue-stability) bash cli for stability.ai API's stable diffusion inference | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/DALL-E.png?raw=1)](https://github.com/kamangir/aiart) tools for AiArt. |
 | [![image](https://github.com/kamangir/awesome-bash-cli/raw/main/assets/marquee.png)](https://github.com/kamangir/awesome-bash-cli) 🚀 a language to speak AI. | [![image](https://user-images.githubusercontent.com/1007567/221448494-d57e08c1-625b-499e-a576-81894f112d6a.jpg)](https://github.com/kamangir/ferfereh) 3d-printed graffiti | [![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/Canadians_v11.gif)](https://github.com/kamangir/Kanata) a multi-screen video feed that is comprised of a matrix of animated faces that slide to the right. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/dec82-6.jpg)](https://github.com/kamangir/dec82) A wearable Raspberry Pi + Grove / Qwiic + Camera. |
 | [![image](https://github.com/kamangir/blue-rvr/raw/master/abcli/assets/marquee.jpeg)](https://github.com/kamangir/blue-rvr) a bash cli for Sphero RVR SDK - runs deep learning vision models on a Raspberry Pi using Python and TensorFlow. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/marquee.jpg)](https://github.com/kamangir/blue-bracket) a parametric 3d-printed bracket to build hardware for machine vision & ai on raspberry pi and jetson nano on the edge. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/blue3-1.jpg)](https://github.com/kamangir/blue-sbc) python + bash bootstrap for edge computing on single board computers. |  |
 
 ---
-built by [`abcli-8.82.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.31.1`](https://github.com/kamangir/kamangir).
+built by [`abcli-8.202.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.38.1`](https://github.com/kamangir/kamangir).
```

