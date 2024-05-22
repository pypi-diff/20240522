# Comparing `tmp/vantage6-node-4.4.1.tar.gz` & `tmp/vantage6-node-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-4.4.1.tar", last modified: Wed May  8 12:54:34 2024, max compression
+gzip compressed data, was "vantage6-node-4.5.0rc3.tar", last modified: Wed May 22 15:04:58 2024, max compression
```

## Comparing `vantage6-node-4.4.1.tar` & `vantage6-node-4.5.0rc3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.696866 vantage6-node-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-08 12:54:34.696866 vantage6-node-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:54:34.696866 vantage6-node-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.692866 vantage6-node-4.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.692866 vantage6-node-4.4.1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.692866 vantage6-node-4.4.1/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    41932 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.692866 vantage6-node-4.4.1/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.696866 vantage6-node-4.4.1/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27826 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/docker/squid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    25123 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    25549 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.696866 vantage6-node-4.4.1/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-08 12:54:22.000000 vantage6-node-4.4.1/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.696866 vantage6-node-4.4.1/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-08 12:54:34.000000 vantage6-node-4.4.1/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-08 12:54:34.000000 vantage6-node-4.4.1/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:34.000000 vantage6-node-4.4.1/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 12:54:34.000000 vantage6-node-4.4.1/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-08 12:54:34.000000 vantage6-node-4.4.1/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 12:54:34.000000 vantage6-node-4.4.1/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    42130 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27837 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25105 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25549 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-4.4.1/PKG-INFO` & `vantage6-node-4.5.0rc3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
@@ -12,47 +12,51 @@
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
 <h3 align=center> A Privacy Enhancing Technology (PET) Operations platform</h3>
 <h3 align="center">
 
 <!-- Badges go here-->
+
 [![Release](https://github.com/vantage6/vantage6/actions/workflows/release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/release.yml)
 [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://badge.fury.io/py/vantage6)
 [![Unittests](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/vantage6/vantage6/badge.svg?branch=main)](https://coveralls.io/github/vantage6/vantage6?branch=main)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://www.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vantage6/vantage6&amp;utm_campaign=Badge_Grade)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://app.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![DOI](https://zenodo.org/badge/492818831.svg)](https://zenodo.org/badge/latestdoi/492818831)
+
 </h3>
 
 <p align="center">
   <a href="#books-quickstart">Quickstart</a> •
   <a href="#project-structure">Project structure</a> •
   <a href="#gift_heart-join-the-community">Join the community</a> •
   <a href="#black_nib-references">References</a>
 </p>
 
+---
 
------------------------------------------------------------------------------------------------------
 This repository is contains all the **vantage6** infrastructure source code. The **vantage6** technology enables to manage and deploy privacy enhancing technologies like Federated Learning (FL) and Multi-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions, suggestions or just want to chat about federated learning: join our [Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel.
 
 ## Infrastructure overview
 
 ![Vantage6 architecture overview](docs/images/overview-infrastructure.png)
 
-*A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network.*
+_A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network._
 
 ## :books: Quickstart
 
 ### Requirements
+
 The **vantage6** infrastructure is delivered in Docker images. To run these images, you need to have [Docker](https://docs.docker.com/get-docker/) installed. To install the latest version of the vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we recommend using an environment manager like [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
 
 Install the latest version of the vantage6 CLI by using:
+
 ```bash
 pip install vantage6
 ```
 
 This install the `v6` commands, which allows you to manage your nodes and servers. To view all available options, run:
 
 ```bash
@@ -79,16 +83,16 @@
 
 # View server logs
 v6 server attach
 ```
 
 From here you can use the [vantage6-client](https://pypi.org/project/vantage6-client) to interact with the server. The demo network has a pre-configured organization with the following credentials:
 
-* Username: `org_1-admin`
-* Password: `password`
+- Username: `org_1-admin`
+- Password: `password`
 
 For example, you can create a new organization by running:
 
 ```python
 from vantage6.client import Client
 
 client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
@@ -106,69 +110,74 @@
 ```
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai)
 
 ## Project structure
 
 ### PYPI packages
+
 This repository is home to 6 PyPi packages:
 
-* [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
-* [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
-* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
-* [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
-* [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
-* [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
-* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
-* [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
+- [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
+- [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+- [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
+- [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
+- [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+- [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
+- [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
+- [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 This repository also hosts the code for the vantage6 user interface (UI). The UI
 is an Angular web application that can be used to interact with the vantage6 server
 easily.
 
 ### Docker images
+
 The vantage6 infrastructure is delivered in Docker images. All Docker images are stored in our private [Harbor](https://goharbor.io/) registry. The most important images are:
 
-* `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
-* `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
-* `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
-* `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
+- `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
+- `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
+- `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
+- `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
 
 with `VERSION` being the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or `4.1.0rc0`.
 
 Several other images are used to support the infrastructure:
 
-* `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
-* `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
-* `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
-* `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
-* `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
-* `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
+- `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
+- `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
+- `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
+- `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
+- `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
+- `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
 
 And finally there are some images released for algorithm development:
 
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
-* `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
 
 ## :gift_heart: Join the community!
+
 We hope to continue developing, improving, and supporting **vantage6** with the help of the federated learning community. If you are interested in contributing, first of all, thank you! Second, please take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/devops/contribute.html)
 
 <a href="https://github.com/vantage6/vantage6/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=vantage6/vantage6" />
 </a>
 
 ## :black_nib: References
+
 If you are using **vantage6**, please cite this repository as well as the accompanying papers as follows:
 
-> * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
-> * A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
-> * D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+> - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
+> - A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
+> - D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+
+---
 
------------------------------------------------------------------------------------------------------
 <p align="center">
   <a href="https://vantage6.ai">vantage6.ai</a> •
   <a href="https://discord.gg/yAyFf6Y">Discord</a> •
   <a href="https://vantage6.discourse.group/">Discourse</a> •
   <a href="https://docs.vantage6.ai">User documentation</a> •
 </p>
```

#### html2text {}

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.4.1 Summary: vantage6 node
-Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.5.0rc3 Summary: vantage6
+node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
    aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//
     vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll)) [[!![[CCoovveerraaggee SSttaattuuss]]((hhttttppss::////
  ccoovveerraallllss..iioo//rreeppooss//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66//bbaaddggee..ssvvgg??bbrraanncchh==mmaaiinn))]]((hhttttppss::////
  ccoovveerraallllss..iioo//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66??bbrraanncchh==mmaaiinn)) [[!![[CCooddaaccyy BBaaddggee]]((hhttttppss::////
 aapppp..ccooddaaccyy..ccoomm//pprroojjeecctt//bbaaddggee//GGrraaddee//22ee6600aacc33bb33ff228844662200880055ff77339999ccbbaa331177bbee))]]((hhttttppss::////
-                     wwwwww..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
-   ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==ggiitthhuubb..ccoomm&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==vvaannttaaggee66//
-   vvaannttaaggee66&&uuttmm__ccaammppaaiiggnn==BBaaddggee__GGrraaddee)) [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//DDOOII//
-   1100..55228811//zzeennooddoo..77338822660022..ssvvgg))]]((hhttttppss::////ddooii..oorrgg//1100..55228811//zzeennooddoo..77338822660022)) ********
+                     aapppp..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
+ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==gghh&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==&&uuttmm__ccaammppaaiiggnn==BBaaddggee__ggrraaddee))
+  [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//449922881188883311..ssvvgg))]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//
+                           llaatteessttddooii//449922881188883311)) ********
     _Q_u_i_c_k_s_t_a_r_t â¢ _P_r_o_j_e_c_t_ _s_t_r_u_c_t_u_r_e â¢ _J_o_i_n_ _t_h_e_ _c_o_m_m_u_n_i_t_y â¢ _R_e_f_e_r_e_n_c_e_s
--------------------------------------------------------------------------------
----------------------- This repository is contains all the **vantage6**
-infrastructure source code. The **vantage6** technology enables to manage and
-deploy privacy enhancing technologies like Federated Learning (FL) and Multi-
-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://
-vantage6.ai) to learn more! You can find more (user) documentation at
-[readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
-questions, suggestions or just want to chat about federated learning: join our
-[Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+--- This repository is contains all the **vantage6** infrastructure source
+code. The **vantage6** technology enables to manage and deploy privacy
+enhancing technologies like Federated Learning (FL) and Multi-Party Computation
+(MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn
+more! You can find more (user) documentation at [readthedocs
+(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
+suggestions or just want to chat about federated learning: join our [Discord
+(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
 Infrastructure overview ![Vantage6 architecture overview](docs/images/overview-
-infrastructure.png) *A High level overview of the vantage6 infrastructure.
+infrastructure.png) _A High level overview of the vantage6 infrastructure.
 Vantage6 has both a client-server and peer-to-peer architecture. The client is
 used by the researcher to create (PET) computation requests. It is also used to
 manage users, organizations and collaborations. The server contains users,
 organizations, collaborations, tasks and their results. It provides a central
 access point for both the clients and nodes. The nodes have access to privacy
 sensitive data and handle computation requests retrieved from the server.
 Computation request are executed as separate containers on the node. These
-containers are connected to containers at other nodes by a VPN network.* ## :
+containers are connected to containers at other nodes by a VPN network._ ## :
 books: Quickstart ### Requirements The **vantage6** infrastructure is delivered
 in Docker images. To run these images, you need to have [Docker](https://
 docs.docker.com/get-docker/) installed. To install the latest version of the
 vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we
 recommend using an environment manager like [mini-conda](https://docs.conda.io/
 en/latest/miniconda.html). Install the latest version of the vantage6 CLI by
 using: ```bash pip install vantage6 ``` This install the `v6` commands, which
@@ -49,75 +48,74 @@
 using: ```bash v6 dev create-demo-network ``` This creates a local network with
 a server and two nodes. You can start the network by running: ```bash v6 dev
 start-demo-network ``` This will start the server and nodes in the background.
 You can view the logs by running: ```bash # View node logs v6 node attach #
 View server logs v6 server attach ``` From here you can use the [vantage6-
 client](https://pypi.org/project/vantage6-client) to interact with the server.
 The demo network has a pre-configured organization with the following
-credentials: * Username: `org_1-admin` * Password: `password` For example, you
+credentials: - Username: `org_1-admin` - Password: `password` For example, you
 can create a new organization by running: ```python from vantage6.client import
 Client client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
 client.authenticate('org_1-admin', 'password') client.setup_encryption(None)
 client.organization.create( name='My organization', address1='My address',
 address2='My address', zipcode='1234AB', country='The Netherlands', domain='my-
 organization.com' ) ``` You can find more (user) documentation at [readthedocs
 (docs.vantage6.ai)](https://docs.vantage6.ai) ## Project structure ### PYPI
-packages This repository is home to 6 PyPi packages: * [vantage6](https://
-pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
+packages This repository is home to 6 PyPi packages: - [vantage6](https://
+pypi.org/project/vantage6) -> _CLI for managing node and server instances_ -
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+for interacting with the vantage6-server_ - [vantage6-algorithm-tools](https://
 pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
-algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
-node) -> _Node application package_ * [vantage6-server](https://pypi.org/
-project/vantage6-server) -> _Server application package_ * [vantage6-algorithm-
+algorithm development_ - [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ - [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ - [vantage6-algorithm-
 store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store
-application package_ * [vantage6-common](https://pypi.org/project/vantage6-
-common) -> _Package with common vantage6 functions_ * [vantage6-backend-common]
+application package_ - [vantage6-common](https://pypi.org/project/vantage6-
+common) -> _Package with common vantage6 functions_ - [vantage6-backend-common]
 (https://pypi.org/project/vantage6-backend-common) -> _Package with functions
 common to central server and algorithm store_ **Note that when using vantage6
 you do not install the _server_ and _node_ packages. These are delivered to you
 in Docker images.** This repository also hosts the code for the vantage6 user
 interface (UI). The UI is an Angular web application that can be used to
 interact with the vantage6 server easily. ### Docker images The vantage6
 infrastructure is delivered in Docker images. All Docker images are stored in
 our private [Harbor](https://goharbor.io/) registry. The most important images
-are: * `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
-Docker image_ * `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
-application Docker image_ * `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
-> _User interface Docker image_ * `harbor2.vantage6.ai/infrastructure/
+are: - `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
+Docker image_ - `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
+application Docker image_ - `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
+> _User interface Docker image_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-store:VERSION` -> _Algorithm store Docker image_ with `VERSION` being
 the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or
-`4.1.0rc0`. Several other images are used to support the infrastructure: *
+`4.1.0rc0`. Several other images are used to support the infrastructure: -
 `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image
-for the infrastructure_ * `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
-> _Squid proxy image used for the whitelisting service_ * `harbor2.vantage6.ai/
-infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ *
+for the infrastructure_ - `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
+> _Squid proxy image used for the whitelisting service_ - `harbor2.vantage6.ai/
+infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ -
 `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect
-to the VPN_ * `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
-image used for initialization_ * `harbor2.vantage6.ai/infrastructure/ssh-
+to the VPN_ - `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
+image used for initialization_ - `harbor2.vantage6.ai/infrastructure/ssh-
 tunnel` -> _SSH tunnel image used for connecting algorithms to external
 services_ And finally there are some images released for algorithm development:
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
-image for algorithm development_ * `harbor2.vantage6.ai/infrastructure/
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
+image for algorithm development_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI
 algorithm development_ ## :gift_heart: Join the community! We hope to continue
 developing, improving, and supporting **vantage6** with the help of the
 federated learning community. If you are interested in contributing, first of
 all, thank you! Second, please take a look at our [contributing guidelines]
 (https://docs.vantage6.ai/en/main/devops/contribute.html) _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_a_n_t_a_g_e_6_/_v_a_n_t_a_g_e_6_]## :black_nib: References If you are
 using **vantage6**, please cite this repository as well as the accompanying
-papers as follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
+papers as follows: > - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
 Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. >
-* A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
+- A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
 VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE
 for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-
 877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-
-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > * D. Smits\*,
+torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > - D. Smits\*,
 B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An
 Improved Infrastructure for Privacy-Preserving Analysis of Patient Data,
 Proceedings of the International Conference of Informatics, Management, and
 Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https:/
 /arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://
-ebooks.iospress.nl/volumearticle/60190)] --------------------------------------
----------------------------------------------------------------
+ebooks.iospress.nl/volumearticle/60190)] ---
        _v_a_n_t_a_g_e_6_._a_i â¢ _D_i_s_c_o_r_d â¢ _D_i_s_c_o_u_r_s_e â¢ _U_s_e_r_ _d_o_c_u_m_e_n_t_a_t_i_o_n â¢
```

### Comparing `vantage6-node-4.4.1/setup.py` & `vantage6-node-4.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/__init__.py` & `vantage6-node-4.5.0rc3/vantage6/node/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
-A node in its simplest would retrieve a task from the central server by
-an API call, run this task and finally return the results to the central
-server again.
+The vantage6 node's core function is to retrieve tasks from the central server, run them
+and return the results.
 
 The node application runs four threads:
 
 *Main thread*
     Checks the task queue and run the next task if there is one available.
 *Listening thread*
     Listens for incoming websocket messages. Among other functionality, it adds
@@ -233,29 +232,29 @@
         log_level = getattr(logging, self.config["logging"]["level"].upper())
         self.proxy_log = get_file_logger(
             "proxy_server", self.ctx.proxy_log_file, log_level_file=log_level
         )
 
         # this is where we try to find a port for the proxyserver
         for try_number in range(5):
-            self.log.info(f"Starting proxyserver at '{proxy_host}:{proxy_port}'")
+            self.log.info("Starting proxyserver at '%s:%s'", proxy_host, proxy_port)
             http_server = WSGIServer(
                 ("0.0.0.0", proxy_port), proxy_server.app, log=self.proxy_log
             )
 
             try:
                 http_server.serve_forever()
 
             except OSError as e:
-                self.log.debug(f"Error during attempt {try_number}")
-                self.log.debug(f"{type(e)}: {e}")
+                self.log.info("Error during attempt %s", try_number)
+                self.log.info("%s: %s", type(e), e)
 
                 if e.errno == 48:
                     proxy_port = random.randint(2048, 16384)
-                    self.log.critical(f"Retrying with a different port: {proxy_port}")
+                    self.log.warning("Retrying with a different port: %s", proxy_port)
                     os.environ["PROXY_SERVER_PORT"] = str(proxy_port)
 
                 else:
                     raise
 
             except Exception as e:
                 self.log.error("Proxyserver could not be started or crashed!")
@@ -263,19 +262,19 @@
 
     def sync_task_queue_with_server(self) -> None:
         """Get all unprocessed tasks from the server for this node."""
         assert self.client.cryptor, "Encrpytion has not been setup"
 
         # request open tasks from the server
         task_results = self.client.run.list(state="open", include_task=True)
-        self.log.debug(task_results)
+        self.log.debug("task_results: %s", task_results)
 
         # add the tasks to the queue
         self.__add_tasks_to_queue(task_results)
-        self.log.info(f"Received {self.queue._qsize()} tasks")
+        self.log.info("Received %s tasks", self.queue._qsize())
 
     def get_task_and_add_to_queue(self, task_id: int) -> None:
         """
         Fetches (open) task with task_id from the server. The `task_id` is
         delivered by the websocket-connection.
 
         Parameters
@@ -418,15 +417,15 @@
             # incoming messages are handled by the action_handler instance
             # which is attached when the socket connection was made. wait()
             # is blocks forever (if no time is specified).
             try:
                 self.socketIO.wait()
             except Exception as e:
                 self.log.error("Listening thread had an exception")
-                self.log.debug(e)
+                self.log.exception(e)
 
     def __speaking_worker(self) -> None:
         """
         Sending messages to central server.
 
         Routine that is in a seperate thread sending results
         to the server when they come available.
@@ -491,25 +490,26 @@
             except Exception:
                 self.log.exception("Speaking thread had an exception")
 
     def __print_connection_error_logs(self):
         """Print error message when node cannot find the server"""
         self.log.warning("Could not connect to the server. Retrying in 10 seconds")
         if self.client.host == "http://localhost" and running_in_docker():
-            self.log.warn(
-                f"You are trying to reach the server at {self.client.host}."
+            self.log.warning(
+                "You are trying to reach the server at %s."
                 " As your node is running inside a Docker container, it cannot"
                 " reach localhost on your host system. Probably, you have to"
                 " change your server URL to http://host.docker.internal (Windows/MacOS)"
                 ' or look into node config option "node_extra_hosts" if using'
-                " http://172.17.0.1 does not work (Linux)."
+                " http://172.17.0.1 does not work (Linux).",
+                self.client.host,
             )
         else:
-            self.log.debug(
-                "Are you sure the server can be reached at " f"{self.client.base_path}?"
+            self.log.info(
+                "Are you sure the server can be reached at %s?", self.client.base_path
             )
 
     def authenticate(self) -> None:
         """
         Authenticate with the server using the api-key from the configuration
         file. If the server rejects for any reason -other than a wrong API key-
         serveral attempts are taken to retry.
@@ -523,26 +523,26 @@
             i = i + 1
             try:
                 self.client.authenticate(api_key)
 
             except AuthenticationException as e:
                 msg = "Authentication failed: API key is wrong!"
                 self.log.warning(msg)
-                self.log.debug(e)
+                self.log.warning(e)
                 break
             except requests.exceptions.ConnectionError:
                 self.__print_connection_error_logs()
                 time.sleep(SLEEP_BTWN_NODE_LOGIN_TRIES)
             except Exception as e:
                 msg = (
                     "Authentication failed. Retrying in "
                     f"{SLEEP_BTWN_NODE_LOGIN_TRIES} seconds!"
                 )
                 self.log.warning(msg)
-                self.log.debug(e)
+                self.log.warning(e)
                 time.sleep(SLEEP_BTWN_NODE_LOGIN_TRIES)
 
             else:
                 # This is only executed if try-block executed without error.
                 success = True
                 break
 
@@ -682,18 +682,16 @@
         )
 
         try:
             squid = Squid(
                 isolated_network_mgr, config, self.ctx.name, volume, custom_squid_image
             )
         except Exception as e:
-            self.log.critical(
-                "Squid proxy failed to initialize. " "Continuing without."
-            )
-            self.log.debug(e, exc_info=True)
+            self.log.critical("Squid proxy failed to initialize. Continuing without.")
+            self.log.exception(e, exc_info=True)
             squid = None
 
         return squid
 
     def setup_ssh_tunnels(
         self, isolated_network_mgr: NetworkManager
     ) -> list[SSHTunnel]:
@@ -856,14 +854,19 @@
                 vpn_manager.connect_vpn()
             except Exception as e:
                 self.log.debug("Could not connect to VPN.")
                 self.log.debug(f"Exception: {e}")
                 # try again in another fashion
                 if next_mode:
                     self._connect_vpn(vpn_manager, next_mode, ovpn_file)
+                else:
+                    self.log.warning(
+                        "Disabling node-to-node communication as VPN "
+                        "connection could not be established."
+                    )
 
     def _get_vpn_config_file(self, ovpn_file: str) -> bool:
         """
         Obtain VPN configuration file from the server
 
         Parameters
         ----------
@@ -975,20 +978,20 @@
                         # triggered, thus break statement is not reached
                         break
 
                     except queue.Empty:
                         pass
 
                     except Exception as e:
-                        self.log.debug(e)
+                        self.log.warning(e)
 
                 if kill_listener.kill_now:
                     raise InterruptedError
 
-                # if task comes available, attempt to execute it
+                # if task becomes available, attempt to execute it
                 try:
                     self.__start_task(taskresult)
                 except Exception as e:
                     self.log.exception(e)
 
         except (KeyboardInterrupt, InterruptedError):
             self.log.info("Node is interrupted, shutting down...")
@@ -1082,15 +1085,15 @@
                     label, type_
                 )
         config_to_share["database_labels"] = labels
         config_to_share["database_types"] = types
         if col_names:
             config_to_share["database_columns"] = col_names
 
-        self.log.debug(f"Sharing node configuration: {config_to_share}")
+        self.log.debug("Sharing node configuration: %s", config_to_share)
         self.socketIO.emit("node_info_update", config_to_share, namespace="/tasks")
 
     def cleanup(self) -> None:
         # TODO add try/catch for all cleanups so that if one fails, the others are
         # still executed
         if hasattr(self, "socketIO") and self.socketIO:
             self.socketIO.disconnect()
```

### Comparing `vantage6-node-4.4.1/vantage6/node/_version.py` & `vantage6-node-4.5.0rc3/vantage6/node/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 4, 1, "final", __build__, 0)
+version_info = (4, 5, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-node-4.4.1/vantage6/node/cli/node.py` & `vantage6-node-4.5.0rc3/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/context.py` & `vantage6-node-4.5.0rc3/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/docker/docker_base.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/docker/docker_manager.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/docker_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
             self.databases[label] = {
                 "uri": uri,
                 "is_file": db_is_file,
                 "type": db_config["type"],
                 "env": db_config.get("env", {}),
             }
-        self.log.debug(f"Databases: {self.databases}")
+        self.log.debug("Databases: %s", self.databases)
 
     def _set_algorithm_device_requests(self, device_requests_config: dict) -> None:
         """
         Configure device access for the algorithm container.
 
         Parameters
         ----------
@@ -268,18 +268,18 @@
         Parameters
         ----------
         volume_name: str
             Name of the volume to be created
         """
         try:
             self.docker.volumes.get(volume_name)
-            self.log.debug(f"Volume {volume_name} already exists.")
+            self.log.debug("Volume %s already exists.", volume_name)
 
         except docker.errors.NotFound:
-            self.log.debug(f"Creating volume {volume_name}")
+            self.log.debug("Creating volume %s", volume_name)
             self.docker.volumes.create(volume_name)
 
     def is_docker_image_allowed(self, docker_image_name: str, task_info: dict) -> bool:
         """
         Checks the docker image name.
 
         Against a list of regular expressions as defined in the configuration
@@ -425,15 +425,15 @@
         Returns
         -------
         list[KilledRun]:
             List of information on tasks that have been killed
         """
         run_ids_killed = []
         if self.active_tasks:
-            self.log.debug(f"Killing {len(self.active_tasks)} active task(s)")
+            self.log.debug("Killing %s active task(s)", len(self.active_tasks))
         while self.active_tasks:
             task = self.active_tasks.pop()
             task.cleanup()
             run_ids_killed.append(
                 KilledRun(
                     run_id=task.run_id, task_id=task.task_id, parent_id=task.parent_id
                 )
@@ -503,16 +503,16 @@
         if not self.is_docker_image_allowed(image, task_info):
             msg = f"Docker image {image} is not allowed on this Node!"
             self.log.critical(msg)
             return TaskStatus.NOT_ALLOWED, None
 
         # Check that this task is not already running
         if self.is_running(run_id):
-            self.log.warn("Task is already being executed, discarding task")
-            self.log.debug(f"run_id={run_id} is discarded")
+            self.log.info("Task is already being executed, discarding task")
+            self.log.debug("run_id=%s is discarded", run_id)
             return TaskStatus.ACTIVE, None
 
         # we pass self.docker instance, in which we may have logged in to registries
         task = DockerTaskManager(
             image=image,
             docker_client=self.docker,
             run_id=run_id,
@@ -598,15 +598,15 @@
             # sleep for a second before checking again
             time.sleep(1)
 
         if finished_tasks:
             # at least one task is finished
 
             finished_task = finished_tasks.pop()
-            self.log.debug(f"Run id={finished_task.run_id} is finished")
+            self.log.debug("Run id=%s is finished", finished_task.run_id)
 
             # Check exit status and report
             logs = finished_task.report_status()
 
             # Cleanup containers
             finished_task.cleanup()
 
@@ -646,16 +646,16 @@
                 self.docker.login(
                     username=registry.get("username"),
                     password=registry.get("password"),
                     registry=registry.get("registry"),
                 )
                 self.log.info(f"Logged in to {registry.get('registry')}")
             except docker.errors.APIError as e:
-                self.log.warn(f"Could not login to {registry.get('registry')}")
-                self.log.debug(e)
+                self.log.warning(f"Could not login to {registry.get('registry')}")
+                self.log.warning(e)
 
     def link_container_to_network(self, container_name: str, config_alias: str) -> None:
         """
         Link a docker container to the isolated docker network
 
         Parameters
         ----------
```

### Comparing `vantage6-node-4.4.1/vantage6/node/docker/exceptions.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/docker/squid.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/squid.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/docker/task_manager.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/task_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,16 @@
         bool:
             True if algorithm container is finished
         """
         try:
             self.container.reload()
         except (docker.errors.NotFound, AttributeError):
             self.log.error("Container not found")
-            self.log.debug(f"- task id: {self.task_id}")
-            self.log.debug(f"- result id: {self.task_id}")
+            self.log.error("- task id: %s", self.task_id)
+            self.log.error("- result id: %s", self.task_id)
             self.status = TaskStatus.UNKNOWN_ERROR
             raise AlgorithmContainerNotFound
 
         return self.container.status == "exited"
 
     def report_status(self) -> str:
         """
@@ -252,15 +252,15 @@
         """
         # generate task folders
         self._make_task_folders()
 
         # prepare volumes
         self.docker_input = docker_input
         self.volumes = self._prepare_volumes(tmp_vol_name, token)
-        self.log.debug(f"volumes: {self.volumes}")
+        self.log.debug("volumes: %s", self.volumes)
 
         # setup environment variables
         self.environment_variables = self._setup_environment_vars(
             algorithm_env=algorithm_env, databases_to_use=databases_to_use
         )
 
         # run the algorithm as docker container
@@ -461,16 +461,16 @@
         dict:
             Environment variables required to run algorithm
         """
         try:
             proxy_host = os.environ["PROXY_SERVER_HOST"]
 
         except Exception:
-            self.log.warn("PROXY_SERVER_HOST not set, using " "host.docker.internal")
-            self.log.debug(os.environ)
+            self.log.warn("PROXY_SERVER_HOST not set, using host.docker.internal")
+            self.log.debug("environment: %s", os.environ)
             proxy_host = "host.docker.internal"
 
         # define environment variables for the docker-container, the
         # host, port and api_path are from the local proxy server to
         # facilitate indirect communication with the central server
         # FIXME: we should only prepend data_folder if database_uri is a
         #   filename
@@ -510,20 +510,20 @@
             environment_variables["no_proxy"] = ", ".join(no_proxy)
 
         for database in databases_to_use:
             if database["label"] not in self.databases:
                 # In this case the algorithm might crash if it tries to access
                 # the DATABASE_LABEL environment variable
                 self.log.warning(
-                    "A user specified a database that does not "
-                    "exist. Available databases are: "
-                    f"{self.databases.keys()}. This is likely to "
-                    "result in an algorithm crash."
+                    "A user specified a database '%s' that does not exist. Available "
+                    "databases are: %s. This is likely to result in an algorithm "
+                    "crash.",
+                    database,
+                    self.databases.keys(),
                 )
-                self.log.debug(f"User specified database: {database}")
             # define env vars for the preprocessing and extra parameters such
             # as query and sheet_name
             extra_params = (
                 json.loads(database.get("parameters"))
                 if database.get("parameters")
                 else {}
             )
```

### Comparing `vantage6-node-4.4.1/vantage6/node/docker/vpn_manager.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/vpn_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/globals.py` & `vantage6-node-4.5.0rc3/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/proxy_server.py` & `vantage6-node-4.5.0rc3/vantage6/node/proxy_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 (!) Not to be confused with the squid proxy that allows algorithm containers
 to access other places in the network.
 """
 
 import requests
 import logging
+import traceback
 
+from time import sleep
 from http import HTTPStatus
 from requests import Response
 
-from flask import Flask, request, jsonify
+from flask import Flask, request
 
 from vantage6.common import bytes_to_base64s, base64s_to_bytes, logger_name
 from vantage6.common.client.node_client import NodeClient
 
 # Initialize FLASK
 app = Flask(__name__)
 log = logging.getLogger(logger_name(__name__))
@@ -42,23 +44,23 @@
     Returns
     -------
     function
         HTTP method
     """
     method_name: str = method.lower()
 
-    loopup = {
+    method_map = {
         "get": requests.get,
         "post": requests.post,
         "patch": requests.patch,
         "put": requests.put,
         "delete": requests.delete,
     }
 
-    return loopup.get(method_name, requests.get)
+    return method_map.get(method_name, requests.get)
 
 
 def make_proxied_request(endpoint: str) -> Response:
     """
     Helper to create proxies requests to the central server.
 
     Parameters
@@ -120,37 +122,45 @@
             # would want to try again
             if response.status_code > 210:
                 log.warning(
                     "Proxy server received status code %s", response.status_code
                 )
                 log.warning("Error messages: %s", response.json())
                 log.debug(
-                    f"method: {request.method}, url: {url}, json: {json}"
-                    f", params: {params}, headers: {headers}"
+                    "method: %s, url: %s, json: %s, params: %s, headers: %s",
+                    request.method,
+                    url,
+                    json,
+                    params,
+                    headers,
                 )
                 if "application/json" in response.headers.get("Content-Type"):
                     log.debug(response.json().get("msg", "no description..."))
 
             else:
                 # Exit the retry loop because we have collected a valid
                 # response
                 return response
 
         except Exception:
             log.exception(
-                f"On attempt {i}, the proxy request raised an " f"exception: <{url}>"
+                "On attempt %s to reach %s, the proxy request raised an exception",
+                i,
+                url,
             )
+            log.debug("Exception details: %s", traceback.format_exc())
+            sleep(1)
 
-    # if all attemps fail, raise an exception to be handled by its parent
+    # if all attempts fail, raise an exception to be handled by its parent
     raise Exception("Proxy request failed")
 
 
 def decrypt_result(run: dict) -> dict:
     """
-    Decrypt the `result` from a run dictonary
+    Decrypt the `result` from a run dictionary
 
     Parameters
     ----------
     run: dict
         Run dict
 
     Returns
@@ -209,35 +219,38 @@
     # We need the server io for the decryption of the results
     client: NodeClient = app.config.get("SERVER_IO")
     if not client:
         log.error(
             "Task proxy request received but proxy server was not "
             "initialized properly."
         )
-        return jsonify({"msg": "Proxy server not initialized properly"}), 500
+        return (
+            {"msg": "Proxy server not initialized properly"},
+            HTTPStatus.INTERNAL_SERVER_ERROR,
+        )
 
     # All requests from algorithms are unencrypted. We encrypt the input
     # field for a specific organization(s) specified by the algorithm
     data = request.get_json()
     organizations = data.get("organizations")
 
     if not organizations:
         log.error("No organizations found in proxy request..")
-        return jsonify({"msg": "Organizations missing from input"}), 400
+        return {"msg": "Organizations missing from input"}, HTTPStatus.BAD_REQUEST
 
     try:
         headers = {"Authorization": request.headers["Authorization"]}
     except Exception:
         log.exception("Could not extract headers from request...")
 
-    log.debug(f"{len(organizations)} organizations")
+    log.debug("%s organizations", len(organizations))
 
     # For every organization we need to encrypt the input field. This is done
     # in parallel as the client (algorithm) is waiting for a timely response.
-    # For every organizationn the public key is retrieved an the input is
+    # For every organization the public key is retrieved an the input is
     # encrypted specifically for them.
     def encrypt_input(organization: dict) -> dict:
         """
         Encrypt the input for a specific organization by using its private key.
         This method is run as background
 
         Parameters
@@ -251,27 +264,27 @@
             Modified organization dictionary in which the `input` key is
             contains encrypted input
         """
         input_ = organization.get("input", {})
         organization_id = organization.get("id")
 
         # retrieve public key of the organization
-        log.debug(f"Retrieving public key of org: {organization_id}")
+        log.debug("Retrieving public key of org: %s", organization_id)
         response = make_request(
             "get", f"organization/{organization_id}", headers=headers
         )
         public_key = response.json().get("public_key")
 
         # Encrypt the input field
         client: NodeClient = app.config.get("SERVER_IO")
         organization["input"] = client.cryptor.encrypt_bytes_to_str(
             base64s_to_bytes(input_), public_key
         )
 
-        log.debug("Input succesfully encrypted for organization " f"{organization_id}!")
+        log.debug("Input succesfully encrypted for organization %s!", organization_id)
         return organization
 
     if client.is_encrypted_collaboration():
         log.debug("Applying end-to-end encryption")
         data["organizations"] = [encrypt_input(o) for o in organizations]
 
     # Attempt to send the task to the central server
@@ -279,15 +292,15 @@
         response = make_request("post", "task", data, headers=headers)
     except Exception:
         log.exception("post task failed")
         return {
             "msg": "Request failed, see node logs"
         }, HTTPStatus.INTERNAL_SERVER_ERROR
 
-    return response.json(), HTTPStatus.OK
+    return response.content, response.status_code, response.headers.items()
 
 
 @app.route("/result", methods=["GET"])
 def proxy_result() -> Response:
     """
     Obtain and decrypt all results to belong to a certain task
 
@@ -295,21 +308,21 @@
     ----------
     id : int
         Task id from which the results need to be obtained
 
     Returns
     -------
     requests.Response
-        Reponse from the vantage6 server
+        Response from the vantage6 server
     """
     # We need the server io for the decryption of the results
     client = app.config.get("SERVER_IO")
     if not client:
         return (
-            jsonify({"msg": "Proxy server not initialized properly"}),
+            {"msg": "Proxy server not initialized properly"},
             HTTPStatus.INTERNAL_SERVER_ERROR,
         )
 
     try:
         task_id = request.args["task_id"]
     except KeyError:
         log.exception("No task id found in request for results...")
@@ -322,21 +335,21 @@
         response: Response = make_proxied_request(f"result?task_id={task_id}")
     except Exception:
         log.exception(f'Error on "result?task_id={task_id}"')
         return {
             "msg": "Request failed, see node logs"
         }, HTTPStatus.INTERNAL_SERVER_ERROR
 
-    # Attempt to decrypt the results. The enpoint should have returned
+    # Attempt to decrypt the results. The endpoint should have returned
     # a list of results
     results = get_response_json_and_handle_exceptions(response)
     for result in results["data"]:
         result = decrypt_result(result)
 
-    return jsonify(results), HTTPStatus.OK
+    return results, response.status_code, response.headers.items()
 
 
 @app.route("/result/<int:id>", methods=["GET"])
 def proxy_results(id_: int) -> Response:
     """
     Obtain and decrypt the algorithm result from the vantage6 server to be used
     by an algorithm container.
@@ -367,15 +380,15 @@
             "msg": "Request failed, see node logs..."
         }, HTTPStatus.INTERNAL_SERVER_ERROR
 
     # Try to decrypt the results
     result = get_response_json_and_handle_exceptions(response)
     result = decrypt_result(result)
 
-    return result, HTTPStatus.OK
+    return result, response.status_code, response.headers.items()
 
 
 @app.route(
     "/<path:central_server_path>", methods=["GET", "POST", "PATCH", "PUT", "DELETE"]
 )
 def proxy(central_server_path: str) -> Response:
     """
```

### Comparing `vantage6-node-4.4.1/vantage6/node/socket.py` & `vantage6-node-4.5.0rc3/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6/node/util/colorer.py` & `vantage6-node-4.5.0rc3/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.4.1/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-4.5.0rc3/vantage6_node.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
@@ -12,47 +12,51 @@
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
 <h3 align=center> A Privacy Enhancing Technology (PET) Operations platform</h3>
 <h3 align="center">
 
 <!-- Badges go here-->
+
 [![Release](https://github.com/vantage6/vantage6/actions/workflows/release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/release.yml)
 [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://badge.fury.io/py/vantage6)
 [![Unittests](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/vantage6/vantage6/badge.svg?branch=main)](https://coveralls.io/github/vantage6/vantage6?branch=main)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://www.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vantage6/vantage6&amp;utm_campaign=Badge_Grade)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://app.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![DOI](https://zenodo.org/badge/492818831.svg)](https://zenodo.org/badge/latestdoi/492818831)
+
 </h3>
 
 <p align="center">
   <a href="#books-quickstart">Quickstart</a> •
   <a href="#project-structure">Project structure</a> •
   <a href="#gift_heart-join-the-community">Join the community</a> •
   <a href="#black_nib-references">References</a>
 </p>
 
+---
 
------------------------------------------------------------------------------------------------------
 This repository is contains all the **vantage6** infrastructure source code. The **vantage6** technology enables to manage and deploy privacy enhancing technologies like Federated Learning (FL) and Multi-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions, suggestions or just want to chat about federated learning: join our [Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel.
 
 ## Infrastructure overview
 
 ![Vantage6 architecture overview](docs/images/overview-infrastructure.png)
 
-*A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network.*
+_A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network._
 
 ## :books: Quickstart
 
 ### Requirements
+
 The **vantage6** infrastructure is delivered in Docker images. To run these images, you need to have [Docker](https://docs.docker.com/get-docker/) installed. To install the latest version of the vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we recommend using an environment manager like [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
 
 Install the latest version of the vantage6 CLI by using:
+
 ```bash
 pip install vantage6
 ```
 
 This install the `v6` commands, which allows you to manage your nodes and servers. To view all available options, run:
 
 ```bash
@@ -79,16 +83,16 @@
 
 # View server logs
 v6 server attach
 ```
 
 From here you can use the [vantage6-client](https://pypi.org/project/vantage6-client) to interact with the server. The demo network has a pre-configured organization with the following credentials:
 
-* Username: `org_1-admin`
-* Password: `password`
+- Username: `org_1-admin`
+- Password: `password`
 
 For example, you can create a new organization by running:
 
 ```python
 from vantage6.client import Client
 
 client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
@@ -106,69 +110,74 @@
 ```
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai)
 
 ## Project structure
 
 ### PYPI packages
+
 This repository is home to 6 PyPi packages:
 
-* [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
-* [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
-* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
-* [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
-* [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
-* [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
-* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
-* [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
+- [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
+- [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+- [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
+- [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
+- [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+- [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
+- [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
+- [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 This repository also hosts the code for the vantage6 user interface (UI). The UI
 is an Angular web application that can be used to interact with the vantage6 server
 easily.
 
 ### Docker images
+
 The vantage6 infrastructure is delivered in Docker images. All Docker images are stored in our private [Harbor](https://goharbor.io/) registry. The most important images are:
 
-* `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
-* `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
-* `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
-* `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
+- `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
+- `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
+- `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
+- `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
 
 with `VERSION` being the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or `4.1.0rc0`.
 
 Several other images are used to support the infrastructure:
 
-* `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
-* `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
-* `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
-* `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
-* `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
-* `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
+- `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
+- `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
+- `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
+- `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
+- `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
+- `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
 
 And finally there are some images released for algorithm development:
 
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
-* `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
 
 ## :gift_heart: Join the community!
+
 We hope to continue developing, improving, and supporting **vantage6** with the help of the federated learning community. If you are interested in contributing, first of all, thank you! Second, please take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/devops/contribute.html)
 
 <a href="https://github.com/vantage6/vantage6/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=vantage6/vantage6" />
 </a>
 
 ## :black_nib: References
+
 If you are using **vantage6**, please cite this repository as well as the accompanying papers as follows:
 
-> * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
-> * A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
-> * D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+> - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
+> - A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
+> - D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+
+---
 
------------------------------------------------------------------------------------------------------
 <p align="center">
   <a href="https://vantage6.ai">vantage6.ai</a> •
   <a href="https://discord.gg/yAyFf6Y">Discord</a> •
   <a href="https://vantage6.discourse.group/">Discourse</a> •
   <a href="https://docs.vantage6.ai">User documentation</a> •
 </p>
```

#### html2text {}

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.4.1 Summary: vantage6 node
-Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.5.0rc3 Summary: vantage6
+node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
    aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//
     vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll)) [[!![[CCoovveerraaggee SSttaattuuss]]((hhttttppss::////
  ccoovveerraallllss..iioo//rreeppooss//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66//bbaaddggee..ssvvgg??bbrraanncchh==mmaaiinn))]]((hhttttppss::////
  ccoovveerraallllss..iioo//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66??bbrraanncchh==mmaaiinn)) [[!![[CCooddaaccyy BBaaddggee]]((hhttttppss::////
 aapppp..ccooddaaccyy..ccoomm//pprroojjeecctt//bbaaddggee//GGrraaddee//22ee6600aacc33bb33ff228844662200880055ff77339999ccbbaa331177bbee))]]((hhttttppss::////
-                     wwwwww..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
-   ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==ggiitthhuubb..ccoomm&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==vvaannttaaggee66//
-   vvaannttaaggee66&&uuttmm__ccaammppaaiiggnn==BBaaddggee__GGrraaddee)) [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//DDOOII//
-   1100..55228811//zzeennooddoo..77338822660022..ssvvgg))]]((hhttttppss::////ddooii..oorrgg//1100..55228811//zzeennooddoo..77338822660022)) ********
+                     aapppp..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
+ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==gghh&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==&&uuttmm__ccaammppaaiiggnn==BBaaddggee__ggrraaddee))
+  [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//449922881188883311..ssvvgg))]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//
+                           llaatteessttddooii//449922881188883311)) ********
     _Q_u_i_c_k_s_t_a_r_t â¢ _P_r_o_j_e_c_t_ _s_t_r_u_c_t_u_r_e â¢ _J_o_i_n_ _t_h_e_ _c_o_m_m_u_n_i_t_y â¢ _R_e_f_e_r_e_n_c_e_s
--------------------------------------------------------------------------------
----------------------- This repository is contains all the **vantage6**
-infrastructure source code. The **vantage6** technology enables to manage and
-deploy privacy enhancing technologies like Federated Learning (FL) and Multi-
-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://
-vantage6.ai) to learn more! You can find more (user) documentation at
-[readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
-questions, suggestions or just want to chat about federated learning: join our
-[Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+--- This repository is contains all the **vantage6** infrastructure source
+code. The **vantage6** technology enables to manage and deploy privacy
+enhancing technologies like Federated Learning (FL) and Multi-Party Computation
+(MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn
+more! You can find more (user) documentation at [readthedocs
+(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
+suggestions or just want to chat about federated learning: join our [Discord
+(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
 Infrastructure overview ![Vantage6 architecture overview](docs/images/overview-
-infrastructure.png) *A High level overview of the vantage6 infrastructure.
+infrastructure.png) _A High level overview of the vantage6 infrastructure.
 Vantage6 has both a client-server and peer-to-peer architecture. The client is
 used by the researcher to create (PET) computation requests. It is also used to
 manage users, organizations and collaborations. The server contains users,
 organizations, collaborations, tasks and their results. It provides a central
 access point for both the clients and nodes. The nodes have access to privacy
 sensitive data and handle computation requests retrieved from the server.
 Computation request are executed as separate containers on the node. These
-containers are connected to containers at other nodes by a VPN network.* ## :
+containers are connected to containers at other nodes by a VPN network._ ## :
 books: Quickstart ### Requirements The **vantage6** infrastructure is delivered
 in Docker images. To run these images, you need to have [Docker](https://
 docs.docker.com/get-docker/) installed. To install the latest version of the
 vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we
 recommend using an environment manager like [mini-conda](https://docs.conda.io/
 en/latest/miniconda.html). Install the latest version of the vantage6 CLI by
 using: ```bash pip install vantage6 ``` This install the `v6` commands, which
@@ -49,75 +48,74 @@
 using: ```bash v6 dev create-demo-network ``` This creates a local network with
 a server and two nodes. You can start the network by running: ```bash v6 dev
 start-demo-network ``` This will start the server and nodes in the background.
 You can view the logs by running: ```bash # View node logs v6 node attach #
 View server logs v6 server attach ``` From here you can use the [vantage6-
 client](https://pypi.org/project/vantage6-client) to interact with the server.
 The demo network has a pre-configured organization with the following
-credentials: * Username: `org_1-admin` * Password: `password` For example, you
+credentials: - Username: `org_1-admin` - Password: `password` For example, you
 can create a new organization by running: ```python from vantage6.client import
 Client client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
 client.authenticate('org_1-admin', 'password') client.setup_encryption(None)
 client.organization.create( name='My organization', address1='My address',
 address2='My address', zipcode='1234AB', country='The Netherlands', domain='my-
 organization.com' ) ``` You can find more (user) documentation at [readthedocs
 (docs.vantage6.ai)](https://docs.vantage6.ai) ## Project structure ### PYPI
-packages This repository is home to 6 PyPi packages: * [vantage6](https://
-pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
+packages This repository is home to 6 PyPi packages: - [vantage6](https://
+pypi.org/project/vantage6) -> _CLI for managing node and server instances_ -
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+for interacting with the vantage6-server_ - [vantage6-algorithm-tools](https://
 pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
-algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
-node) -> _Node application package_ * [vantage6-server](https://pypi.org/
-project/vantage6-server) -> _Server application package_ * [vantage6-algorithm-
+algorithm development_ - [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ - [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ - [vantage6-algorithm-
 store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store
-application package_ * [vantage6-common](https://pypi.org/project/vantage6-
-common) -> _Package with common vantage6 functions_ * [vantage6-backend-common]
+application package_ - [vantage6-common](https://pypi.org/project/vantage6-
+common) -> _Package with common vantage6 functions_ - [vantage6-backend-common]
 (https://pypi.org/project/vantage6-backend-common) -> _Package with functions
 common to central server and algorithm store_ **Note that when using vantage6
 you do not install the _server_ and _node_ packages. These are delivered to you
 in Docker images.** This repository also hosts the code for the vantage6 user
 interface (UI). The UI is an Angular web application that can be used to
 interact with the vantage6 server easily. ### Docker images The vantage6
 infrastructure is delivered in Docker images. All Docker images are stored in
 our private [Harbor](https://goharbor.io/) registry. The most important images
-are: * `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
-Docker image_ * `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
-application Docker image_ * `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
-> _User interface Docker image_ * `harbor2.vantage6.ai/infrastructure/
+are: - `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
+Docker image_ - `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
+application Docker image_ - `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
+> _User interface Docker image_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-store:VERSION` -> _Algorithm store Docker image_ with `VERSION` being
 the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or
-`4.1.0rc0`. Several other images are used to support the infrastructure: *
+`4.1.0rc0`. Several other images are used to support the infrastructure: -
 `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image
-for the infrastructure_ * `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
-> _Squid proxy image used for the whitelisting service_ * `harbor2.vantage6.ai/
-infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ *
+for the infrastructure_ - `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
+> _Squid proxy image used for the whitelisting service_ - `harbor2.vantage6.ai/
+infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ -
 `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect
-to the VPN_ * `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
-image used for initialization_ * `harbor2.vantage6.ai/infrastructure/ssh-
+to the VPN_ - `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
+image used for initialization_ - `harbor2.vantage6.ai/infrastructure/ssh-
 tunnel` -> _SSH tunnel image used for connecting algorithms to external
 services_ And finally there are some images released for algorithm development:
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
-image for algorithm development_ * `harbor2.vantage6.ai/infrastructure/
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
+image for algorithm development_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI
 algorithm development_ ## :gift_heart: Join the community! We hope to continue
 developing, improving, and supporting **vantage6** with the help of the
 federated learning community. If you are interested in contributing, first of
 all, thank you! Second, please take a look at our [contributing guidelines]
 (https://docs.vantage6.ai/en/main/devops/contribute.html) _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_a_n_t_a_g_e_6_/_v_a_n_t_a_g_e_6_]## :black_nib: References If you are
 using **vantage6**, please cite this repository as well as the accompanying
-papers as follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
+papers as follows: > - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
 Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. >
-* A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
+- A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
 VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE
 for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-
 877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-
-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > * D. Smits\*,
+torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > - D. Smits\*,
 B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An
 Improved Infrastructure for Privacy-Preserving Analysis of Patient Data,
 Proceedings of the International Conference of Informatics, Management, and
 Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https:/
 /arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://
-ebooks.iospress.nl/volumearticle/60190)] --------------------------------------
----------------------------------------------------------------
+ebooks.iospress.nl/volumearticle/60190)] ---
        _v_a_n_t_a_g_e_6_._a_i â¢ _D_i_s_c_o_r_d â¢ _D_i_s_c_o_u_r_s_e â¢ _U_s_e_r_ _d_o_c_u_m_e_n_t_a_t_i_o_n â¢
```

### Comparing `vantage6-node-4.4.1/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-4.5.0rc3/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

