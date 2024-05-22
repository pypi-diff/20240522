# Comparing `tmp/ipython-ngql-0.9.0.tar.gz` & `tmp/ipython-ngql-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-ngql-0.9.0.tar", last modified: Wed Apr  3 10:59:17 2024, max compression
+gzip compressed data, was "ipython-ngql-0.9.1.tar", last modified: Thu Apr  4 03:34:30 2024, max compression
```

## Comparing `ipython-ngql-0.9.0.tar` & `ipython-ngql-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/ipython_ngql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 10:59:17.000000 ipython-ngql-0.9.0/ipython_ngql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:59:17.459383 ipython-ngql-0.9.0/ngql/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/ngql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35833 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/ngql/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:59:17.463383 ipython-ngql-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 10:59:12.000000 ipython-ngql-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:34:30.014948 ipython-ngql-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 03:34:25.000000 ipython-ngql-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-04 03:34:30.014948 ipython-ngql-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-04 03:34:25.000000 ipython-ngql-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:34:30.014948 ipython-ngql-0.9.1/ipython_ngql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-04 03:34:30.000000 ipython-ngql-0.9.1/ipython_ngql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 03:34:30.000000 ipython-ngql-0.9.1/ipython_ngql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:34:30.000000 ipython-ngql-0.9.1/ipython_ngql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 03:34:30.000000 ipython-ngql-0.9.1/ipython_ngql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 03:34:30.000000 ipython-ngql-0.9.1/ipython_ngql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:34:30.014948 ipython-ngql-0.9.1/ngql/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 03:34:25.000000 ipython-ngql-0.9.1/ngql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36253 2024-04-04 03:34:25.000000 ipython-ngql-0.9.1/ngql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:34:30.014948 ipython-ngql-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-04 03:34:25.000000 ipython-ngql-0.9.1/setup.py
```

### Comparing `ipython-ngql-0.9.0/LICENSE` & `ipython-ngql-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython-ngql-0.9.0/PKG-INFO` & `ipython-ngql-0.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: ipython-ngql
-Version: 0.9.0
-Summary: Jupyter and iPython extension for NebulaGraph
-Home-page: https://github.com/wey-gu/ipython-ngql
+Version: 0.9.1
+Summary: Jupyter extension for NebulaGraph
+Home-page: https://github.com/wey-gu/jupyter_nebulagraph
 Author: Wey Gu
 Author-email: weyl.gu@gmail.com
-Project-URL: Bug Tracker, https://github.com/wey-gu/ipython-ngql/issues
+Project-URL: Bug Tracker, https://github.com/wey-gu/jupyter_nebulagraph/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jinja2
 Requires-Dist: nebula3-python>=3.5.0
 Requires-Dist: pandas
+Requires-Dist: tqdm
+Requires-Dist: pyvis
 
 
-[![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/ipython-ngql?label=Version)](https://github.com/wey-gu/ipython-ngql/releases)
-[![pypi-version](https://img.shields.io/pypi/v/ipython-ngql)](https://pypi.org/project/ipython-ngql/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb)
+[![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
+[![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
 
-https://github.com/wey-gu/ipython-ngql/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
-
-`ipython-ngql` is a Python package for connecting to NebulaGraph in Jupyter Notebook or iPython. It simplifies creating, debugging, and sharing Jupyter Notebooks with NebulaGraph interactions for better collaboration.
+https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
+`jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
 Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
 
 ![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
 ![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
 
 ## Get Started
 
-Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb).
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
+
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
-`ipython-ngql` could be installed either via pip or from this git repo itself.
+`jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
 ```bash
-pip install ipython-ngql
+pip install jupyter_nebulagraph
 ```
 
 > Install inside the repo
 
 ```bash
-git clone git@github.com:wey-gu/ipython-ngql.git
-cd ipython-ngql
+git clone git@github.com:wey-gu/jupyter_nebulagraph.git
+cd jupyter_nebulagraph
 python setup.py install
 ```
 
 ### Load it in Jupyter Notebook or iPython
 
 ```python
 %load_ext ngql
@@ -98,15 +101,15 @@
 SHOW HOSTS;
 ```
 
 > There will be other options in future, i.e. from a `.ngql` file.
 
 ### Query String with Variables
 
-`ipython-ngql` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
+`jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
 In [8]: vid = "player100"
 
 In [9]: %%ngql
@@ -130,23 +133,23 @@
 %ng_draw
 
 # another query
 %ngql match p=(:player)-[]->() return p LIMIT 5
 %ng_draw
 ```
 
-![](https://github.com/wey-gu/ipython-ngql/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
+![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
 
 ### Draw Graph Schema
 
 ```python
 %ng_draw_schema
 ```
 
-![](https://github.com/wey-gu/ipython-ngql/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
+![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
 
 ### Load Data from CSV
 
 It's supported to load data from a CSV file into NebulaGraph with the help of `ng_load_csv` magic.
 
 For example, to load data from a CSV file `actor.csv` into a space `basketballplayer` with tag `player` and vid in column `0`, and props in column `1` and `2`:
 
@@ -162,24 +165,24 @@
 %ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer
 ```
 
 Some other examples:
 
 ```python
 # load CSV from a URL
-%ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer -b 2
+%ng_load --source https://github.com/wey-gu/jupyter_nebulagraph/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer
 # with rank column
 %ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
 # without rank column
 %ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
 ```
 
 ### Configure `ngql_result_style`
 
-By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
+By default, `jupyter_nebulagraph` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
 %config IPythonNGQL.ngql_result_style="raw"
 ```
 
@@ -240,15 +243,15 @@
 In [1]: %ngql help
 ```
 
 ### Examples
 
 #### Jupyter Notebook
 
-Please refer here:https://github.com/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
 In [1]: %load_ext ngql
 
 In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
```

### Comparing `ipython-ngql-0.9.0/README.md` & `ipython-ngql-0.9.1/ipython_ngql.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,65 @@
+Metadata-Version: 2.1
+Name: ipython-ngql
+Version: 0.9.1
+Summary: Jupyter extension for NebulaGraph
+Home-page: https://github.com/wey-gu/jupyter_nebulagraph
+Author: Wey Gu
+Author-email: weyl.gu@gmail.com
+Project-URL: Bug Tracker, https://github.com/wey-gu/jupyter_nebulagraph/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Jinja2
+Requires-Dist: nebula3-python>=3.5.0
+Requires-Dist: pandas
+Requires-Dist: tqdm
+Requires-Dist: pyvis
+
+
+[![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
+[![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
-[![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/ipython-ngql?label=Version)](https://github.com/wey-gu/ipython-ngql/releases)
-[![pypi-version](https://img.shields.io/pypi/v/ipython-ngql)](https://pypi.org/project/ipython-ngql/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb)
 
-
-https://github.com/wey-gu/ipython-ngql/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
-
-`ipython-ngql` is a Python package for connecting to NebulaGraph in Jupyter Notebook or iPython. It simplifies creating, debugging, and sharing Jupyter Notebooks with NebulaGraph interactions for better collaboration.
+https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
+`jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
 Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
 
 ![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
 ![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
 
 ## Get Started
 
-Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb).
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
+
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
-`ipython-ngql` could be installed either via pip or from this git repo itself.
+`jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
 ```bash
-pip install ipython-ngql
+pip install jupyter_nebulagraph
 ```
 
 > Install inside the repo
 
 ```bash
-git clone git@github.com:wey-gu/ipython-ngql.git
-cd ipython-ngql
+git clone git@github.com:wey-gu/jupyter_nebulagraph.git
+cd jupyter_nebulagraph
 python setup.py install
 ```
 
 ### Load it in Jupyter Notebook or iPython
 
 ```python
 %load_ext ngql
@@ -80,15 +101,15 @@
 SHOW HOSTS;
 ```
 
 > There will be other options in future, i.e. from a `.ngql` file.
 
 ### Query String with Variables
 
-`ipython-ngql` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
+`jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
 In [8]: vid = "player100"
 
 In [9]: %%ngql
@@ -112,23 +133,23 @@
 %ng_draw
 
 # another query
 %ngql match p=(:player)-[]->() return p LIMIT 5
 %ng_draw
 ```
 
-![](https://github.com/wey-gu/ipython-ngql/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
+![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
 
 ### Draw Graph Schema
 
 ```python
 %ng_draw_schema
 ```
 
-![](https://github.com/wey-gu/ipython-ngql/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
+![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
 
 ### Load Data from CSV
 
 It's supported to load data from a CSV file into NebulaGraph with the help of `ng_load_csv` magic.
 
 For example, to load data from a CSV file `actor.csv` into a space `basketballplayer` with tag `player` and vid in column `0`, and props in column `1` and `2`:
 
@@ -144,24 +165,24 @@
 %ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer
 ```
 
 Some other examples:
 
 ```python
 # load CSV from a URL
-%ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer -b 2
+%ng_load --source https://github.com/wey-gu/jupyter_nebulagraph/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer
 # with rank column
 %ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
 # without rank column
 %ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
 ```
 
 ### Configure `ngql_result_style`
 
-By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
+By default, `jupyter_nebulagraph` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
 %config IPythonNGQL.ngql_result_style="raw"
 ```
 
@@ -222,15 +243,15 @@
 In [1]: %ngql help
 ```
 
 ### Examples
 
 #### Jupyter Notebook
 
-Please refer here:https://github.com/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
 In [1]: %load_ext ngql
 
 In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
```

### Comparing `ipython-ngql-0.9.0/ipython_ngql.egg-info/PKG-INFO` & `ipython-ngql-0.9.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,45 @@
-Metadata-Version: 2.1
-Name: ipython-ngql
-Version: 0.9.0
-Summary: Jupyter and iPython extension for NebulaGraph
-Home-page: https://github.com/wey-gu/ipython-ngql
-Author: Wey Gu
-Author-email: weyl.gu@gmail.com
-Project-URL: Bug Tracker, https://github.com/wey-gu/ipython-ngql/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Jinja2
-Requires-Dist: nebula3-python>=3.5.0
-Requires-Dist: pandas
-
-
-[![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/ipython-ngql?label=Version)](https://github.com/wey-gu/ipython-ngql/releases)
-[![pypi-version](https://img.shields.io/pypi/v/ipython-ngql)](https://pypi.org/project/ipython-ngql/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb)
 
+[![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
+[![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
-https://github.com/wey-gu/ipython-ngql/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
 
-`ipython-ngql` is a Python package for connecting to NebulaGraph in Jupyter Notebook or iPython. It simplifies creating, debugging, and sharing Jupyter Notebooks with NebulaGraph interactions for better collaboration.
+https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
+`jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
 Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
 
 ![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
 ![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
 
 ## Get Started
 
-Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb).
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
+
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
-`ipython-ngql` could be installed either via pip or from this git repo itself.
+`jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
 ```bash
-pip install ipython-ngql
+pip install jupyter_nebulagraph
 ```
 
 > Install inside the repo
 
 ```bash
-git clone git@github.com:wey-gu/ipython-ngql.git
-cd ipython-ngql
+git clone git@github.com:wey-gu/jupyter_nebulagraph.git
+cd jupyter_nebulagraph
 python setup.py install
 ```
 
 ### Load it in Jupyter Notebook or iPython
 
 ```python
 %load_ext ngql
@@ -98,15 +81,15 @@
 SHOW HOSTS;
 ```
 
 > There will be other options in future, i.e. from a `.ngql` file.
 
 ### Query String with Variables
 
-`ipython-ngql` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
+`jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
 In [8]: vid = "player100"
 
 In [9]: %%ngql
@@ -130,23 +113,23 @@
 %ng_draw
 
 # another query
 %ngql match p=(:player)-[]->() return p LIMIT 5
 %ng_draw
 ```
 
-![](https://github.com/wey-gu/ipython-ngql/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
+![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
 
 ### Draw Graph Schema
 
 ```python
 %ng_draw_schema
 ```
 
-![](https://github.com/wey-gu/ipython-ngql/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
+![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/81fd71b5-61e7-4c65-93be-c2f4e507611b)
 
 ### Load Data from CSV
 
 It's supported to load data from a CSV file into NebulaGraph with the help of `ng_load_csv` magic.
 
 For example, to load data from a CSV file `actor.csv` into a space `basketballplayer` with tag `player` and vid in column `0`, and props in column `1` and `2`:
 
@@ -162,24 +145,24 @@
 %ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer
 ```
 
 Some other examples:
 
 ```python
 # load CSV from a URL
-%ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer -b 2
+%ng_load --source https://github.com/wey-gu/jupyter_nebulagraph/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer
 # with rank column
 %ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
 # without rank column
 %ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
 ```
 
 ### Configure `ngql_result_style`
 
-By default, `ipython-ngql` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
+By default, `jupyter_nebulagraph` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
 
 This can be done ad-hoc with below one line:
 
 ```python
 %config IPythonNGQL.ngql_result_style="raw"
 ```
 
@@ -240,15 +223,15 @@
 In [1]: %ngql help
 ```
 
 ### Examples
 
 #### Jupyter Notebook
 
-Please refer here:https://github.com/wey-gu/ipython-ngql/blob/main/examples/get_started.ipynb
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
 
 #### iPython
 
 ```python
 In [1]: %load_ext ngql
 
 In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
```

### Comparing `ipython-ngql-0.9.0/ngql/magic.py` & `ipython-ngql-0.9.1/ngql/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from IPython.core.magic import (
     Magics,
     magics_class,
     line_cell_magic,
     needs_local_scope,
 )
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
+from tqdm.notebook import tqdm
 
 from typing import Dict, List
 import networkx as nx
 
 
 from jinja2 import Template, Environment, meta
 from traitlets.config.configurable import Configurable
@@ -326,15 +327,15 @@
         "player999","player1000",50,1
 
         %ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
 
         #follow.csv
         "player999","player1000",50
 
-        %ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer -b 2
+        %ng_load --source https://github.com/wey-gu/ipython-ngql/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer
 
 
         """
         print(help_info)
         return
 
     @needs_local_scope
@@ -855,15 +856,17 @@
         QUOTE = '"'
 
         if args.tag:
             # Load vertex_data into NebulaGraph under the specified tag and space
             # Now prepare INSERT query for vertices in batches
             # Example of QUERY: INSERT VERTEX t2 (name, age) VALUES "13":("n3", 12), "14":("n4", 8);
 
-            for i in range(0, len(vertex_data), batch_size):
+            for i in tqdm(
+                range(0, len(vertex_data), batch_size), desc="Loading Vertices"
+            ):
                 batch = vertex_data.iloc[i : i + batch_size]
                 query = f"INSERT VERTEX {args.tag} ({', '.join([col for col in vertex_data.columns if col != '___vid'])}) VALUES "
                 for index, row in batch.iterrows():
                     vid_str = f'{QUOTE_VID}{row["___vid"]}{QUOTE_VID}'
                     prop_str = ""
                     if with_props:
                         for prop_name in props_mapping.values():
@@ -885,26 +888,27 @@
                 try:
                     result = self._execute(query)
                 except Exception as e:
                     print(
                         f"INSERT Failed on row {i + index}, data: {row}, error: {result.error_msg()}"
                     )
                     return
+                tqdm.write(f"Loaded {i + len(batch)} of {len(vertex_data)} vertices")
 
             print(
                 f"Successfully loaded {len(vertex_data)} vertices '{args.space}' for tag '{args.tag}'"
             )
         elif args.edge:
             # Load edge_data into NebulaGraph under the specified edge type and space
             # Now prepare INSERT query for edges in batches
             # Example of QUERY:
             # with_rank INSERT EDGE e1 (name, age) VALUES "13" -> "14"@1:("n3", 12), "14" -> "15"@132:("n4", 8);
             # without_rank INSERT EDGE e1 (name, age) VALUES "13" -> "14":("n3", 12), "14" -> "15":("n4", 8);
 
-            for i in range(0, len(edge_data), batch_size):
+            for i in tqdm(range(0, len(edge_data), batch_size), desc="Loading Edges"):
                 batch = edge_data.iloc[i : i + batch_size]
                 query = f"INSERT EDGE {args.edge} ({', '.join([col for col in edge_data.columns if col not in ['___src', '___dst', '___rank']])}) VALUES "
                 for index, row in batch.iterrows():
                     src_str = f'{QUOTE_VID}{row["___src"]}{QUOTE_VID}'
                     dst_str = f'{QUOTE_VID}{row["___dst"]}{QUOTE_VID}'
                     prop_str = ""
                     if with_props:
@@ -931,7 +935,11 @@
                 try:
                     result = self._execute(query)
                 except Exception as e:
                     print(
                         f"INSERT Failed on row {i + index}, data: {row}, error: {result.error_msg()}"
                     )
                     return
+                tqdm.write(f"Loaded {i + len(batch)} of {len(edge_data)} edges")
+            print(
+                f"Successfully loaded {len(edge_data)} edges '{args.space}' for edge type '{args.edge}'"
+            )
```

### Comparing `ipython-ngql-0.9.0/setup.py` & `ipython-ngql-0.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipython-ngql",
-    version="0.9.0",
+    version="0.9.1",
     author="Wey Gu",
     author_email="weyl.gu@gmail.com",
-    description="Jupyter and iPython extension for NebulaGraph",
+    description="Jupyter extension for NebulaGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/wey-gu/ipython-ngql",
+    url="https://github.com/wey-gu/jupyter_nebulagraph",
     project_urls={
-        "Bug Tracker": "https://github.com/wey-gu/ipython-ngql/issues",
+        "Bug Tracker": "https://github.com/wey-gu/jupyter_nebulagraph/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     install_requires=[
         "Jinja2",
         "nebula3-python>=3.5.0",
         "pandas",
+        "tqdm",
+        "pyvis",
     ],
 )
```

