# Comparing `tmp/kamangir-3.41.1.tar.gz` & `tmp/kamangir-3.47.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kamangir-3.41.1.tar", last modified: Wed May 22 02:19:10 2024, max compression
+gzip compressed data, was "kamangir-3.47.1.tar", last modified: Wed May 22 02:28:51 2024, max compression
```

## Comparing `kamangir-3.41.1.tar` & `kamangir-3.47.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:19:10.723890 kamangir-3.41.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.41.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:43.000000 kamangir-3.41.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-22 02:19:10.723425 kamangir-3.41.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3243 2024-05-21 02:52:53.000000 kamangir-3.41.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:19:10.720869 kamangir-3.41.1/kamangir/
--rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-22 02:19:04.000000 kamangir-3.41.1/kamangir/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4623 2024-05-22 02:18:49.000000 kamangir-3.41.1/kamangir/content.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-21 02:51:14.000000 kamangir-3.41.1/kamangir/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:19:10.722896 kamangir-3.41.1/kamangir.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     3408 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      303 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-22 02:19:10.000000 kamangir-3.41.1/kamangir.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      430 2024-05-22 02:17:19.000000 kamangir-3.41.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-22 02:19:10.723987 kamangir-3.41.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      488 2024-05-20 01:29:24.000000 kamangir-3.41.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:28:51.924437 kamangir-3.47.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.47.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:43.000000 kamangir-3.47.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     3965 2024-05-22 02:28:51.923818 kamangir-3.47.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3243 2024-05-22 02:28:32.000000 kamangir-3.47.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:28:51.920153 kamangir-3.47.1/kamangir/
+-rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-22 02:28:46.000000 kamangir-3.47.1/kamangir/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-05-21 02:51:14.000000 kamangir-3.47.1/kamangir/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4623 2024-05-22 02:18:49.000000 kamangir-3.47.1/kamangir/content.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-05-21 02:51:14.000000 kamangir-3.47.1/kamangir/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-21 02:51:14.000000 kamangir-3.47.1/kamangir/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-21 02:51:14.000000 kamangir-3.47.1/kamangir/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-22 02:28:51.923059 kamangir-3.47.1/kamangir.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3965 2024-05-22 02:28:51.000000 kamangir-3.47.1/kamangir.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      349 2024-05-22 02:28:51.000000 kamangir-3.47.1/kamangir.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-22 02:28:51.000000 kamangir-3.47.1/kamangir.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-22 02:28:51.000000 kamangir-3.47.1/kamangir.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-22 02:28:51.000000 kamangir-3.47.1/kamangir.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-22 02:19:52.000000 kamangir-3.47.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      430 2024-05-22 02:17:19.000000 kamangir-3.47.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-22 02:28:51.924578 kamangir-3.47.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-22 02:20:30.000000 kamangir-3.47.1/setup.py
```

### Comparing `kamangir-3.41.1/LICENSE` & `kamangir-3.47.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kamangir-3.41.1/PKG-INFO` & `kamangir-3.47.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-Metadata-Version: 2.1
-Name: kamangir
-Version: 3.41.1
-Summary: kamangir.net
-Author: arash@kamangir.net
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 My name is [Arash](http://kamangir.net/); I mix [ai](https://github.com/kamangir/roofAI), [cloud](https://github.com/kamangir/hubble), and [mathematics](https://github.com/kamangir/giza) into minimal forms that seek survival.
 
 
 | [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks and scripts for ai experiments and aws batch jobs. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 a recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
 | --- | --- | --- | --- |
 | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/carrot.png)](https://github.com/kamangir/openai_cli) 🛠️ tools for the OpenAI API | [![image](https://github.com/kamangir/hubble/raw/main/assets/hst/u4ge0106r_c0m.gif)](https://github.com/kamangir/hubble) 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry. | [![image](https://github.com/kamangir/AI-ART/raw/main/blue-stability/blue_stability.gif)](https://github.com/kamangir/blue-stability) bash cli for stability.ai API's stable diffusion inference | [![image](https://github.com/kamangir/openai_cli/raw/main/assets/DALL-E.png?raw=1)](https://github.com/kamangir/aiart) tools for AiArt. |
 | [![image](https://github.com/kamangir/awesome-bash-cli/raw/main/assets/marquee.png)](https://github.com/kamangir/awesome-bash-cli) 🚀 a language to speak AI. | [![image](https://user-images.githubusercontent.com/1007567/221448494-d57e08c1-625b-499e-a576-81894f112d6a.jpg)](https://github.com/kamangir/ferfereh) 3d-printed graffiti | [![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/Canadians_v11.gif)](https://github.com/kamangir/Kanata) a multi-screen video feed that is comprised of a matrix of animated faces that slide to the right. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/dec82-6.jpg)](https://github.com/kamangir/dec82) A wearable Raspberry Pi + Grove / Qwiic + Camera. |
 | [![image](https://github.com/kamangir/blue-rvr/raw/master/abcli/assets/marquee.jpeg)](https://github.com/kamangir/blue-rvr) a bash cli for Sphero RVR SDK - runs deep learning vision models on a Raspberry Pi using Python and TensorFlow. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/marquee.jpg)](https://github.com/kamangir/blue-bracket) a parametric 3d-printed bracket to build hardware for machine vision & ai on raspberry pi and jetson nano on the edge. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/blue3-1.jpg)](https://github.com/kamangir/blue-sbc) python + bash bootstrap for edge computing on single board computers. |  |
 
 ---
-built by [`abcli-8.202.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.38.1`](https://github.com/kamangir/kamangir).
+built by [`abcli-8.208.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.46.1`](https://github.com/kamangir/kamangir).
```

### Comparing `kamangir-3.41.1/kamangir/__main__.py` & `kamangir-3.47.1/kamangir/__main__.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.41.1/kamangir/content.py` & `kamangir-3.47.1/kamangir/content.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.41.1/kamangir/functions.py` & `kamangir-3.47.1/kamangir/functions.py`

 * *Files identical despite different names*

