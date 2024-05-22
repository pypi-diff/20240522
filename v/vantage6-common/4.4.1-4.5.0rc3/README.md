# Comparing `tmp/vantage6-common-4.4.1.tar.gz` & `tmp/vantage6-common-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-4.4.1.tar", last modified: Wed May  8 12:54:32 2024, max compression
+gzip compressed data, was "vantage6-common-4.5.0rc3.tar", last modified: Wed May 22 15:04:56 2024, max compression
```

## Comparing `vantage6-common-4.4.1.tar` & `vantage6-common-4.5.0rc3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:32.980870 vantage6-common-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-08 12:54:32.980870 vantage6-common-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:54:32.980870 vantage6-common-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:32.976870 vantage6-common-4.4.1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:32.980870 vantage6-common-4.4.1/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:32.980870 vantage6-common-4.4.1/vantage6/common/client/
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/client/client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/client/node_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:32.980870 vantage6-common-4.4.1/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-08 12:54:22.000000 vantage6-common-4.4.1/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:32.980870 vantage6-common-4.4.1/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-08 12:54:32.000000 vantage6-common-4.4.1/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-08 12:54:32.000000 vantage6-common-4.4.1/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:32.000000 vantage6-common-4.4.1/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 12:54:32.000000 vantage6-common-4.4.1/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 12:54:32.000000 vantage6-common-4.4.1/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.885278 vantage6-common-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:56.885278 vantage6-common-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:56.885278 vantage6-common-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.877278 vantage6-common-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6/common/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    19098 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-22 15:04:46.000000 vantage6-common-4.5.0rc3/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:56.881278 vantage6-common-4.5.0rc3/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:04:56.000000 vantage6-common-4.5.0rc3/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-4.4.1/PKG-INFO` & `vantage6-common-4.5.0rc3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 common
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
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.4.1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.5.0rc3 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
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

### Comparing `vantage6-common-4.4.1/setup.py` & `vantage6-common-4.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/__init__.py` & `vantage6-common-4.5.0rc3/vantage6/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Common functionality used in multiple vantage6 components.
+"""
+
 import os
 import base64
 import click
 import appdirs
 import ipaddress
 import typing
 import uuid
```

### Comparing `vantage6-common-4.4.1/vantage6/common/_version.py` & `vantage6-common-4.5.0rc3/vantage6/common/_version.py`

 * *Files 17% similar despite different names*

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

### Comparing `vantage6-common-4.4.1/vantage6/common/client/client_base.py` & `vantage6-common-4.5.0rc3/vantage6/common/client/client_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,29 +244,29 @@
                 timeout_attempts += 1
                 if (
                     attempts_on_timeout is not None
                     and timeout_attempts > attempts_on_timeout
                 ):
                     return {"msg": "Connection error"}
                 self.log.error("Connection error... Retrying")
-                self.log.debug(exc)
+                self.log.info(exc)
                 time.sleep(1)
 
         # TODO: should check for a non 2xx response
         if response.status_code > 210:
             self.log.error(f"Server responded with error code: {response.status_code}")
             try:
                 self.log.error(
                     "msg: %s. Endpoint: %s", response.json().get("msg", ""), endpoint
                 )
                 if response.json().get("errors"):
                     self.log.error("errors:" + str(response.json().get("errors")))
             except json_lib.JSONDecodeError:
                 self.log.error("Did not find a message from the server")
-                self.log.debug(response.content)
+                self.log.error(response.content)
 
             if retry:
                 if first_try:
                     self.refresh_token()
                     return self.request(
                         endpoint,
                         json,
@@ -377,17 +377,29 @@
             self.log.debug(f"Authenticating user {credentials['username']}...")
         elif "api_key" in credentials:
             self.log.debug("Authenticating node...")
 
         # authenticate to the central server
         url = self.generate_path_to(path, is_for_algorithm_store=False)
         response = requests.post(url, json=credentials)
-        data = response.json()
+        if response.status_code == 404:
+            self.log.error(
+                "Server not found at %s. Please check the address and whether the "
+                "server is running!",
+                url,
+            )
+            self.log.info(
+                "If the server is running and reachable, %s/health should give a "
+                "response.",
+                self.base_path,
+            )
+            return False
 
         # handle negative responses
+        data = response.json()
         if response.status_code > 200:
             self.log.critical(f"Failed to authenticate: {data.get('msg')}")
             if response.status_code == 401:
                 raise AuthenticationException("Failed to authenticate")
             else:
                 raise Exception("Failed to authenticate")
 
@@ -470,15 +482,15 @@
         try:
             # TODO this only works when the runs belong to the
             # same organization... We should make different implementation
             # of get_results
             input_ = cryptor.decrypt_str_to_bytes(input_)
 
         except Exception as e:
-            self.log.debug(e)
+            self.log.exception(e)
 
         return input_
 
     def _decrypt_field(self, data: dict, field: str, is_single_resource: bool) -> dict:
         """
         Wrapper function to decrypt and deserialize the a field of one or more
         resources
```

### Comparing `vantage6-common-4.4.1/vantage6/common/client/node_client.py` & `vantage6-common-4.5.0rc3/vantage6/common/client/node_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         Returns
         -------
         dict
             The container token.
         """
         self.log.debug(
-            f"requesting container token for task_id={task_id} " f"and image={image}"
+            "Requesting container token for task_id=%s and image=%s", task_id, image
         )
         return self.request(
             "/token/container", method="post", json={"task_id": task_id, "image": image}
         )
 
     class Run(ClientBase.SubClient):
         """Subclient for the run endpoint."""
@@ -148,16 +148,16 @@
             if include_task:
                 params["include"] = "task"
             if task_id:
                 params["task_id"] = task_id
             run_data = self.parent.request(endpoint="run", params=params)
 
             if isinstance(run_data, str):
-                self.parent.log.warn("Requesting algorithm runs failed")
-                self.parent.log.debug(f"Fail message: {run_data}")
+                self.parent.log.warning("Requesting algorithm runs failed")
+                self.parent.log.warning(f"Fail message: {run_data}")
                 return {}
 
             # if there are multiple pages of algorithm runs, get them all
             links = run_data.get("links")
             page = 1
             while links and links.get("next"):
                 page += 1
```

### Comparing `vantage6-common-4.4.1/vantage6/common/client/utils.py` & `vantage6-common-4.5.0rc3/vantage6/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/colors.py` & `vantage6-common-4.5.0rc3/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/configuration_manager.py` & `vantage6-common-4.5.0rc3/vantage6/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/context.py` & `vantage6-common-4.5.0rc3/vantage6/common/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/docker/addons.py` & `vantage6-common-4.5.0rc3/vantage6/common/docker/addons.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 def check_docker_running() -> None:
     """
     Check if docker engine is running. If not, exit the program.
     """
     try:
         docker_client = docker.from_env()
         docker_client.ping()
-    except Exception as e:
+    except Exception as exc:
         log.error(
             "Cannot reach the Docker engine! Please make sure Docker " "is running."
         )
-        log.warn("Exiting...")
-        log.debug(e)
+        log.exception(exc)
+        log.warning("Exiting...")
         exit(1)
 
 
 def running_in_docker() -> bool:
     """
     Check if this code is executed within a Docker container.
 
@@ -78,18 +78,18 @@
     ------
     docker.errors.APIError
         If the image could not be pulled
     """
     try:
         docker_client.images.pull(image)
         log.debug("Succeeded to pull image %s", image)
-    except docker.errors.APIError as e:
+    except docker.errors.APIError as exc:
         log.error("Failed to pull image! %s", image)
-        log.error(e)
-        raise docker.errors.APIError("Failed to pull image") from e
+        log.exception(exc)
+        raise docker.errors.APIError("Failed to pull image") from exc
 
 
 def get_container(docker_client: DockerClient, **filters) -> Container:
     """
     Return container if it exists after searching using kwargs
 
     Parameters
@@ -140,15 +140,15 @@
     kill: bool
         Whether or not container should be killed before it is removed
     """
     try:
         container.remove(force=kill)
     except Exception as e:
         log.exception(f"Failed to remove container {container.name}")
-        log.debug(e)
+        log.exception(e)
 
 
 def stop_container(container: Container, force: bool = False):
     """
     Stop a docker container
 
     Parameters
@@ -297,8 +297,8 @@
         Volume to delete
     """
     try:
         volume = client.volumes.get(volume_name)
         if volume:
             volume.remove()
     except (docker.errors.NotFound, docker.errors.APIError):
-        log.warning("Could not delete volume %s", volume.name)
+        log.warning("Could not delete volume %s", volume_name)
```

### Comparing `vantage6-common-4.4.1/vantage6/common/docker/network_manager.py` & `vantage6-common-4.5.0rc3/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/encryption.py` & `vantage6-common-4.5.0rc3/vantage6/common/encryption.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 it using the public key of the receiving organization. (retreiving
 these public keys is outside the scope of this module).
 """
 
 # TODO handle no public key from other organization (should that happen here?)
 import os
 import logging
+import json
 
 from pathlib import Path
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
@@ -276,36 +277,39 @@
 
         Returns
         -------
         str
             The encrypted data encoded as base64 string.
         """
 
-        # Use the shared key for symmetric encryption/decryption of the payload
+        # Use the shared key for symmetric encryption of the payload
         shared_key = os.urandom(32)
         iv_bytes = os.urandom(16)
 
+        # encrypt the data symmetrically with the shared key. This is done because
+        # symmetric encryption is faster than asymmetric encryption and results in a
+        # smaller result.
         cipher = Cipher(
             algorithms.AES(shared_key), modes.CTR(iv_bytes), backend=default_backend()
         )
-
         encryptor = cipher.encryptor()
         encrypted_msg_bytes = encryptor.update(data) + encryptor.finalize()
 
         # Create a public key instance.
         pubkey = load_pem_public_key(
             base64s_to_bytes(pubkey_base64s), backend=default_backend()
         )
 
+        # Encrypt the shared key using the public key (i.e. assymmetrically)
         encrypted_key_bytes = pubkey.encrypt(shared_key, padding.PKCS1v15())
 
+        # Join the encrypted key, iv and encrypted message into a single string
         encrypted_key = self.bytes_to_str(encrypted_key_bytes)
         iv = self.bytes_to_str(iv_bytes)
         encrypted_msg = self.bytes_to_str(encrypted_msg_bytes)
-
         return SEPARATOR.join([encrypted_key, iv, encrypted_msg])
 
     def decrypt_str_to_bytes(self, data: str) -> bytes:
         """
         Decrypt base64 encoded *string* data.
 
         Parameters
@@ -314,35 +318,56 @@
             The data to decrypt.
 
         Returns
         -------
         bytes
             The decrypted data.
         """
-
+        # Note that the decryption process is the reverse of the encryption process
+        # in the function above
         (encrypted_key, iv, encrypted_msg) = data.split(SEPARATOR)
 
-        # Yes, this can be done more efficiently.
+        # Convert the strings to back to bytes
         encrypted_key_bytes = self.str_to_bytes(encrypted_key)
         iv_bytes = self.str_to_bytes(iv)
         encrypted_msg_bytes = self.str_to_bytes(encrypted_msg)
 
         # Decrypt the shared key using asymmetric encryption
         shared_key = self.private_key.decrypt(encrypted_key_bytes, padding.PKCS1v15())
 
-        self.log.debug("Decrypted shared key: %s", shared_key)
+        # In the UI, the bytes have to be base64 encoded before encryption (we cannot
+        # encrypt bytes directly in javascript) - so if this key was encrypted in the
+        # UI, we need to decode it here as extra step. If it fails, ignore it as it is
+        # apparently not needed.
+        # TODO v5+ add additional encoding step in Python so that we always have the
+        # same process
+        try:
+            shared_key = base64s_to_bytes(shared_key.decode("utf-8"))
+        except UnicodeDecodeError:
+            pass
 
-        # Use the shared key for symmetric encryption/decryption of the payload
+        # Use the shared key for symmetric decryption of the payload
         cipher = Cipher(
             algorithms.AES(shared_key), modes.CTR(iv_bytes), backend=default_backend()
         )
-
         decryptor = cipher.decryptor()
         result = decryptor.update(encrypted_msg_bytes) + decryptor.finalize()
 
+        # In the UI, the result has an extra base64 encoding step also for the
+        # symmetrical part of the encryption. If it fails, ignore it as it is
+        # apparently not needed.
+        # TODO v5+ adapt as stated above in decrypting shared key
+        try:
+            json.loads(result.decode("utf-8"))
+        except json.decoder.JSONDecodeError:
+            try:
+                result = base64s_to_bytes(result.decode("utf-8"))
+            except UnicodeDecodeError:
+                pass
+
         return result
 
     def verify_public_key(self, pubkey_base64: str) -> bool:
         """
         Verifies the public key.
 
         Compare a public key with the generated public key from the private key
```

### Comparing `vantage6-common-4.4.1/vantage6/common/globals.py` & `vantage6-common-4.5.0rc3/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/log.py` & `vantage6-common-4.5.0rc3/vantage6/common/log.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/serialization.py` & `vantage6-common-4.5.0rc3/vantage6/common/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/task_status.py` & `vantage6-common-4.5.0rc3/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6/common/utest.py` & `vantage6-common-4.5.0rc3/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.4.1/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-4.5.0rc3/vantage6_common.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 common
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
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.4.1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.5.0rc3 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
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

### Comparing `vantage6-common-4.4.1/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-4.5.0rc3/vantage6_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

