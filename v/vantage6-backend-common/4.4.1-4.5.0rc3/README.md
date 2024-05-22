# Comparing `tmp/vantage6-backend-common-4.4.1.tar.gz` & `tmp/vantage6-backend-common-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-backend-common-4.4.1.tar", last modified: Wed May  8 12:54:35 2024, max compression
+gzip compressed data, was "vantage6-backend-common-4.5.0rc3.tar", last modified: Wed May 22 15:04:59 2024, max compression
```

## Comparing `vantage6-backend-common-4.4.1.tar` & `vantage6-backend-common-4.5.0rc3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/vantage6/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/vantage6/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/vantage6/backend/common/__build__
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/vantage6/backend/common/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/vantage6/backend/common/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/vantage6/backend/common/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/vantage6/backend/common/resource/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/vantage6/backend/common/resource/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/vantage6/backend/common/services_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 12:54:22.000000 vantage6-backend-common-4.4.1/vantage6/backend/common/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.080865 vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-08 12:54:35.000000 vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-08 12:54:35.000000 vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:35.000000 vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 12:54:35.000000 vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 12:54:35.000000 vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/services_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 15:04:46.000000 vantage6-backend-common-4.5.0rc3/vantage6/backend/common/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.137293 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:04:59.000000 vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/top_level.txt
```

### Comparing `vantage6-backend-common-4.4.1/PKG-INFO` & `vantage6-backend-common-4.5.0rc3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-backend-common
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 common backend functionalities
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.4.1 Summary:
+Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.5.0rc3 Summary:
 Vantage6 common backend functionalities Home-page: https://github.com/vantage6/
 vantage6 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
@@ -10,38 +10,37 @@
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
@@ -50,75 +49,74 @@
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

### Comparing `vantage6-backend-common-4.4.1/setup.py` & `vantage6-backend-common-4.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.4.1/vantage6/backend/common/_version.py` & `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/_version.py`

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

### Comparing `vantage6-backend-common-4.4.1/vantage6/backend/common/resource/output_schema.py` & `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/output_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.4.1/vantage6/backend/common/resource/pagination.py` & `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/resource/pagination.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.4.1/vantage6/backend/common/services_resources.py` & `vantage6-backend-common-4.5.0rc3/vantage6/backend/common/services_resources.py`

 * *Files identical despite different names*

### Comparing `vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/PKG-INFO` & `vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-backend-common
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 common backend functionalities
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.4.1 Summary:
+Metadata-Version: 2.1 Name: vantage6-backend-common Version: 4.5.0rc3 Summary:
 Vantage6 common backend functionalities Home-page: https://github.com/vantage6/
 vantage6 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
@@ -10,38 +10,37 @@
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
@@ -50,75 +49,74 @@
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

### Comparing `vantage6-backend-common-4.4.1/vantage6_backend_common.egg-info/SOURCES.txt` & `vantage6-backend-common-4.5.0rc3/vantage6_backend_common.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 setup.py
 vantage6/backend/common/__build__
+vantage6/backend/common/__init__.py
 vantage6/backend/common/_version.py
 vantage6/backend/common/globals.py
 vantage6/backend/common/services_resources.py
 vantage6/backend/common/session.py
 vantage6/backend/common/resource/output_schema.py
 vantage6/backend/common/resource/pagination.py
 vantage6_backend_common.egg-info/PKG-INFO
```

