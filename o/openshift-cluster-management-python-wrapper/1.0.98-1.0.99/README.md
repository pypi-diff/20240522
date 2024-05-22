# Comparing `tmp/openshift_cluster_management_python_wrapper-1.0.98.tar.gz` & `tmp/openshift_cluster_management_python_wrapper-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_cluster_management_python_wrapper-1.0.98.tar", max compression
+gzip compressed data, was "openshift_cluster_management_python_wrapper-1.0.99.tar", max compression
```

## Comparing `openshift_cluster_management_python_wrapper-1.0.98.tar` & `openshift_cluster_management_python_wrapper-1.0.99.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-08 07:25:15.322684 openshift_cluster_management_python_wrapper-1.0.98/LICENSE
--rw-r--r--   0        0        0     1346 2024-04-08 07:25:15.322684 openshift_cluster_management_python_wrapper-1.0.98/README.md
--rw-r--r--   0        0        0        0 2024-04-08 07:25:15.322684 openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/__init__.py
--rw-r--r--   0        0        0    33804 2024-04-08 07:25:15.322684 openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/cluster.py
--rw-r--r--   0        0        0      554 2024-04-08 07:25:15.323684 openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/exceptions.py
--rw-r--r--   0        0        0      882 2024-04-08 07:25:15.323684 openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/manifests/managed-api-service-policy.json
--rw-r--r--   0        0        0     4139 2024-04-08 07:25:15.323684 openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/ocm_client.py
--rw-r--r--   0        0        0     1405 2024-04-08 07:25:15.323684 openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/versions.py
--rw-r--r--   0        0        0     1927 2024-04-08 07:25:19.824653 openshift_cluster_management_python_wrapper-1.0.98/pyproject.toml
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 openshift_cluster_management_python_wrapper-1.0.98/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 14:09:12.056741 openshift_cluster_management_python_wrapper-1.0.99/LICENSE
+-rw-r--r--   0        0        0     1346 2024-04-08 14:09:12.056741 openshift_cluster_management_python_wrapper-1.0.99/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 14:09:12.057741 openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/__init__.py
+-rw-r--r--   0        0        0    33804 2024-04-08 14:09:12.057741 openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/cluster.py
+-rw-r--r--   0        0        0      554 2024-04-08 14:09:12.057741 openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/exceptions.py
+-rw-r--r--   0        0        0      882 2024-04-08 14:09:12.057741 openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/manifests/managed-api-service-policy.json
+-rw-r--r--   0        0        0     4139 2024-04-08 14:09:12.057741 openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/ocm_client.py
+-rw-r--r--   0        0        0     1405 2024-04-08 14:09:12.057741 openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/versions.py
+-rw-r--r--   0        0        0     1927 2024-04-08 14:09:16.624709 openshift_cluster_management_python_wrapper-1.0.99/pyproject.toml
+-rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 openshift_cluster_management_python_wrapper-1.0.99/PKG-INFO
```

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/LICENSE` & `openshift_cluster_management_python_wrapper-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/README.md` & `openshift_cluster_management_python_wrapper-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/cluster.py` & `openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/exceptions.py` & `openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/manifests/managed-api-service-policy.json` & `openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/manifests/managed-api-service-policy.json`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/ocm_client.py` & `openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/ocm_client.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/ocm_python_wrapper/versions.py` & `openshift_cluster_management_python_wrapper-1.0.99/ocm_python_wrapper/versions.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/pyproject.toml` & `openshift_cluster_management_python_wrapper-1.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "openshift-cluster-management-python-wrapper"
 description = "Wrapper around https://github.com/openshift/openshift-cluster-management-python-client"
-version = "1.0.98"
+version = "1.0.99"
 authors = ["Meni Yakove <myakove@gmail.com>", "Ruth Netser <rnetser@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/RedHatQE/openshift-cluster-management-python-wrapper"
 documentation = "https://github.com/RedHatQE/openshift-cluster-management-python-wrapper/blob/main/README.md"
 keywords = ["Openshift", "OCM"]
 classifiers = [
```

### Comparing `openshift_cluster_management_python_wrapper-1.0.98/PKG-INFO` & `openshift_cluster_management_python_wrapper-1.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-wrapper
-Version: 1.0.98
+Version: 1.0.99
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Home-page: https://github.com/RedHatQE/openshift-cluster-management-python-wrapper
 License: Apache-2.0
 Keywords: Openshift,OCM
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
```

