# Comparing `tmp/openshift_cli_installer-2.0.8.tar.gz` & `tmp/openshift_cli_installer-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_cli_installer-2.0.8.tar", max compression
+gzip compressed data, was "openshift_cli_installer-2.0.9.tar", max compression
```

## Comparing `openshift_cli_installer-2.0.8.tar` & `openshift_cli_installer-2.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-12-19 09:00:53.793111 openshift_cli_installer-2.0.8/LICENSE
--rw-r--r--   0        0        0    12778 2023-12-19 09:00:53.794111 openshift_cli_installer-2.0.8/README.md
--rw-r--r--   0        0        0        0 2023-12-19 09:00:53.794111 openshift_cli_installer-2.0.8/openshift_cli_installer/__init__.py
--rw-r--r--   0        0        0     7476 2023-12-19 09:00:53.794111 openshift_cli_installer-2.0.8/openshift_cli_installer/cli.py
--rw-r--r--   0        0        0        0 2023-12-19 09:00:53.794111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/__init__.py
--rw-r--r--   0        0        0        0 2023-12-19 09:00:53.794111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/__init__.py
--rw-r--r--   0        0        0     7149 2023-12-19 09:00:53.794111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/aws_ipi_cluster.py
--rw-r--r--   0        0        0     2669 2023-12-19 09:00:53.794111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/ocm_cluster.py
--rw-r--r--   0        0        0    19167 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/ocp_cluster.py
--rw-r--r--   0        0        0     8395 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/ocp_clusters.py
--rw-r--r--   0        0        0     4520 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/osd_cluster.py
--rw-r--r--   0        0        0    11800 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/rosa_cluster.py
--rw-r--r--   0        0        0    15416 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/libs/user_input.py
--rw-r--r--   0        0        0     2689 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/manifests/clusters.example.yaml
--rw-r--r--   0        0        0      845 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/manifests/install-config-template.j2
--rw-r--r--   0        0        0     1346 2023-12-19 09:00:53.795111 openshift_cli_installer-2.0.8/openshift_cli_installer/manifests/setup-vpc.tf
--rw-r--r--   0        0        0     2724 2023-12-19 09:00:53.796111 openshift_cli_installer-2.0.8/openshift_cli_installer/scripts/openshift-cli-installer-build-command.py
--rw-r--r--   0        0        0        0 2023-12-19 09:00:53.796111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/__init__.py
--rw-r--r--   0        0        0   304655 2023-12-19 09:00:53.797111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/all_aws_versions.json
--rw-r--r--   0        0        0     9647 2023-12-19 09:00:53.797111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/all_osd_versions.py
--rw-r--r--   0        0        0     7063 2023-12-19 09:00:53.797111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/all_rosa_versions.py
--rw-r--r--   0        0        0      998 2023-12-19 09:00:53.797111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/test_build_command_script.py
--rw-r--r--   0        0        0     9356 2023-12-19 09:00:53.797111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/test_cluster_version.py
--rw-r--r--   0        0        0     1923 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/test_user_input.py
--rw-r--r--   0        0        0      722 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/tests/utils.py
--rw-r--r--   0        0        0        0 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/utils/__init__.py
--rw-r--r--   0        0        0     1094 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/utils/cli_utils.py
--rw-r--r--   0        0        0     2879 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/utils/click_dict_type.py
--rw-r--r--   0        0        0     7104 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/utils/cluster_versions.py
--rw-r--r--   0        0        0     6564 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/utils/clusters.py
--rw-r--r--   0        0        0      983 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/utils/const.py
--rw-r--r--   0        0        0     4266 2023-12-19 09:00:53.798111 openshift_cli_installer-2.0.8/openshift_cli_installer/utils/general.py
--rw-r--r--   0        0        0     1713 2023-12-19 09:00:59.075085 openshift_cli_installer-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    14468 1970-01-01 00:00:00.000000 openshift_cli_installer-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-09 11:21:35.152931 openshift_cli_installer-2.0.9/LICENSE
+-rw-r--r--   0        0        0    12778 2024-01-09 11:21:35.153931 openshift_cli_installer-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-09 11:21:35.153931 openshift_cli_installer-2.0.9/openshift_cli_installer/__init__.py
+-rw-r--r--   0        0        0     7476 2024-01-09 11:21:35.153931 openshift_cli_installer-2.0.9/openshift_cli_installer/cli.py
+-rw-r--r--   0        0        0        0 2024-01-09 11:21:35.153931 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-09 11:21:35.153931 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/__init__.py
+-rw-r--r--   0        0        0     7149 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/aws_ipi_cluster.py
+-rw-r--r--   0        0        0     2669 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/ocm_cluster.py
+-rw-r--r--   0        0        0    19161 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/ocp_cluster.py
+-rw-r--r--   0        0        0     8395 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/ocp_clusters.py
+-rw-r--r--   0        0        0     4520 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/osd_cluster.py
+-rw-r--r--   0        0        0    11800 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/rosa_cluster.py
+-rw-r--r--   0        0        0    15416 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/libs/user_input.py
+-rw-r--r--   0        0        0     2689 2024-01-09 11:21:35.154930 openshift_cli_installer-2.0.9/openshift_cli_installer/manifests/clusters.example.yaml
+-rw-r--r--   0        0        0      845 2024-01-09 11:21:35.155930 openshift_cli_installer-2.0.9/openshift_cli_installer/manifests/install-config-template.j2
+-rw-r--r--   0        0        0     1346 2024-01-09 11:21:35.155930 openshift_cli_installer-2.0.9/openshift_cli_installer/manifests/setup-vpc.tf
+-rw-r--r--   0        0        0     2724 2024-01-09 11:21:35.155930 openshift_cli_installer-2.0.9/openshift_cli_installer/scripts/openshift-cli-installer-build-command.py
+-rw-r--r--   0        0        0        0 2024-01-09 11:21:35.155930 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/__init__.py
+-rw-r--r--   0        0        0   304655 2024-01-09 11:21:35.156931 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/all_aws_versions.json
+-rw-r--r--   0        0        0     9647 2024-01-09 11:21:35.156931 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/all_osd_versions.py
+-rw-r--r--   0        0        0     7063 2024-01-09 11:21:35.156931 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/all_rosa_versions.py
+-rw-r--r--   0        0        0      998 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/test_build_command_script.py
+-rw-r--r--   0        0        0     9356 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/test_cluster_version.py
+-rw-r--r--   0        0        0     1923 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/test_user_input.py
+-rw-r--r--   0        0        0      722 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/utils/__init__.py
+-rw-r--r--   0        0        0     1094 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/utils/cli_utils.py
+-rw-r--r--   0        0        0     2879 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/utils/click_dict_type.py
+-rw-r--r--   0        0        0     7104 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/utils/cluster_versions.py
+-rw-r--r--   0        0        0     6564 2024-01-09 11:21:35.157930 openshift_cli_installer-2.0.9/openshift_cli_installer/utils/clusters.py
+-rw-r--r--   0        0        0      983 2024-01-09 11:21:35.158930 openshift_cli_installer-2.0.9/openshift_cli_installer/utils/const.py
+-rw-r--r--   0        0        0     4266 2024-01-09 11:21:35.158930 openshift_cli_installer-2.0.9/openshift_cli_installer/utils/general.py
+-rw-r--r--   0        0        0     1740 2024-01-09 11:21:40.152883 openshift_cli_installer-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    14516 1970-01-01 00:00:00.000000 openshift_cli_installer-2.0.9/PKG-INFO
```

### Comparing `openshift_cli_installer-2.0.8/LICENSE` & `openshift_cli_installer-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/README.md` & `openshift_cli_installer-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/cli.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/cli.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/aws_ipi_cluster.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/aws_ipi_cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/ocm_cluster.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/ocm_cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/ocp_cluster.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/ocp_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ocp_resources.cluster_version import ClusterVersion
 from ocp_resources.managed_cluster import ManagedCluster
 from ocp_resources.multi_cluster_hub import MultiClusterHub
 from ocp_resources.multi_cluster_observability import MultiClusterObservability
 from ocp_resources.namespace import Namespace
 from ocp_resources.route import Route
 from ocp_resources.secret import Secret
-from ocp_resources.utils import TimeoutWatch
+from timeout_sampler import TimeoutWatch
 from ocp_utilities.infra import get_client
 from ocp_utilities.must_gather import run_must_gather
 from ocp_utilities.utils import run_command
 from simple_logger.logger import get_logger
 
 from openshift_cli_installer.libs.user_input import UserInput
 from openshift_cli_installer.utils.cluster_versions import (
@@ -251,17 +251,17 @@
         if self.cluster_object:
             self.ocp_client = self.cluster_object.ocp_client
             self.cluster_info["cluster-id"] = self.cluster_object.cluster_id
 
         else:
             self.ocp_client = get_client(config_file=self.cluster_info["kubeconfig-path"])
             # Unmanaged clusters name is set to cluster id
-            self.cluster_info["cluster-id"] = self.cluster_info["display-name"] = (
-                ClusterVersion(client=self.ocp_client, name="version").instance.spec.clusterID
-            )
+            self.cluster_info["cluster-id"] = self.cluster_info["display-name"] = ClusterVersion(
+                client=self.ocp_client, name="version"
+            ).instance.spec.clusterID
 
         self.cluster_info["api-url"] = self.ocp_client.configuration.host
         console_route = Route(name="console", namespace="openshift-console", client=self.ocp_client)
         if console_route.exists:
             route_spec = console_route.instance.spec
             self.cluster_info["console-url"] = f"{route_spec.port.targetPort}://{route_spec.host}"
```

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/ocp_clusters.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/ocp_clusters.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/osd_cluster.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/osd_cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/libs/clusters/rosa_cluster.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/libs/clusters/rosa_cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/libs/user_input.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/libs/user_input.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/manifests/clusters.example.yaml` & `openshift_cli_installer-2.0.9/openshift_cli_installer/manifests/clusters.example.yaml`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/manifests/install-config-template.j2` & `openshift_cli_installer-2.0.9/openshift_cli_installer/manifests/install-config-template.j2`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/manifests/setup-vpc.tf` & `openshift_cli_installer-2.0.9/openshift_cli_installer/manifests/setup-vpc.tf`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/scripts/openshift-cli-installer-build-command.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/scripts/openshift-cli-installer-build-command.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/tests/all_aws_versions.json` & `openshift_cli_installer-2.0.9/openshift_cli_installer/tests/all_aws_versions.json`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/tests/all_osd_versions.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/tests/all_osd_versions.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/tests/all_rosa_versions.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/tests/all_rosa_versions.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/tests/test_build_command_script.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/tests/test_build_command_script.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/tests/test_cluster_version.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/tests/test_cluster_version.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/tests/test_user_input.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/tests/test_user_input.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/tests/utils.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/utils/cli_utils.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/utils/click_dict_type.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/utils/click_dict_type.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/utils/cluster_versions.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/utils/cluster_versions.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/utils/clusters.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/utils/clusters.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/utils/const.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/utils/const.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/openshift_cli_installer/utils/general.py` & `openshift_cli_installer-2.0.9/openshift_cli_installer/utils/general.py`

 * *Files identical despite different names*

### Comparing `openshift_cli_installer-2.0.8/pyproject.toml` & `openshift_cli_installer-2.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "openshift-cli-installer"
-version = "2.0.8"
+version = "2.0.9"
 description = "CLI to install/uninstall Openshift clusters."
 readme = "README.md"
 repository = "https://github.com/RedHatQE/openshift-cli-installer"
 authors = ["Meni Yakove <myakove@gmail.com>", "Ruth Netser <rnetser@gmail.com>"]
 license = "Apache-2.0"
 packages = [{ include = "openshift_cli_installer" }]
 include = [{ path = "manifests/*" }]
@@ -41,14 +41,15 @@
 openshift-python-utilities = "^5.0.0"
 pyaml-env = "^1.2.1"
 google-cloud-compute = "^1.14.1"
 redhat-qe-cloud-tools = "^1.0.19"
 python-simple-logger = "^1.0.7"
 ipdb = "^0.13.13"
 ruff = "^0.1.5"
+timeout-sampler = "^0.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ipython = "*"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `openshift_cli_installer-2.0.8/PKG-INFO` & `openshift_cli_installer-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cli-installer
-Version: 2.0.8
+Version: 2.0.9
 Summary: CLI to install/uninstall Openshift clusters.
 Home-page: https://github.com/RedHatQE/openshift-cli-installer
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,14 +27,15 @@
 Requires-Dist: python-simple-logger (>=1.0.7,<2.0.0)
 Requires-Dist: python-terraform (>=0.10.1,<0.11.0)
 Requires-Dist: redhat-qe-cloud-tools (>=1.0.19,<2.0.0)
 Requires-Dist: rosa-python-client (>=1.0.36,<2.0.0)
 Requires-Dist: ruff (>=0.1.5,<0.2.0)
 Requires-Dist: semver (>=3.0.1,<4.0.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
+Requires-Dist: timeout-sampler (>=0.0.1,<0.0.2)
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-cli-installer/blob/main/README.md
 Project-URL: Repository, https://github.com/RedHatQE/openshift-cli-installer
 Description-Content-Type: text/markdown
 
 # openshift-cli-installer
 Basic Openshift install CLI wrapper.  
 The tool allows deploying or deletion of one or more clusters.
```

