# Comparing `tmp/openshift_python_utilities-5.0.8.tar.gz` & `tmp/openshift_python_utilities-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_python_utilities-5.0.8.tar", max compression
+gzip compressed data, was "openshift_python_utilities-5.0.9.tar", max compression
```

## Comparing `openshift_python_utilities-5.0.8.tar` & `openshift_python_utilities-5.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-11-20 13:28:20.178611 openshift_python_utilities-5.0.8/LICENSE
--rw-r--r--   0        0        0      745 2023-11-20 13:28:20.178611 openshift_python_utilities-5.0.8/README.md
--rw-r--r--   0        0        0        0 2023-11-20 13:28:20.178611 openshift_python_utilities-5.0.8/ocp_utilities/__init__.py
--rw-r--r--   0        0        0      495 2023-11-20 13:28:20.178611 openshift_python_utilities-5.0.8/ocp_utilities/debugger.py
--rw-r--r--   0        0        0      452 2023-11-20 13:28:20.178611 openshift_python_utilities-5.0.8/ocp_utilities/exceptions.py
--rw-r--r--   0        0        0    13542 2023-11-20 13:28:20.178611 openshift_python_utilities-5.0.8/ocp_utilities/infra.py
--rw-r--r--   0        0        0     7502 2023-11-20 13:28:20.179611 openshift_python_utilities-5.0.8/ocp_utilities/monitoring.py
--rw-r--r--   0        0        0     1877 2023-11-20 13:28:20.179611 openshift_python_utilities-5.0.8/ocp_utilities/must_gather.py
--rw-r--r--   0        0        0    14091 2023-11-20 13:28:20.179611 openshift_python_utilities-5.0.8/ocp_utilities/operators.py
--rw-r--r--   0        0        0     3445 2023-11-20 13:28:20.179611 openshift_python_utilities-5.0.8/ocp_utilities/utils.py
--rw-r--r--   0        0        0     1546 2023-11-20 13:28:24.939569 openshift_python_utilities-5.0.8/pyproject.toml
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 openshift_python_utilities-5.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-27 14:22:26.066259 openshift_python_utilities-5.0.9/LICENSE
+-rw-r--r--   0        0        0      745 2023-11-27 14:22:26.066259 openshift_python_utilities-5.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-11-27 14:22:26.066259 openshift_python_utilities-5.0.9/ocp_utilities/__init__.py
+-rw-r--r--   0        0        0      495 2023-11-27 14:22:26.066259 openshift_python_utilities-5.0.9/ocp_utilities/debugger.py
+-rw-r--r--   0        0        0      452 2023-11-27 14:22:26.066259 openshift_python_utilities-5.0.9/ocp_utilities/exceptions.py
+-rw-r--r--   0        0        0    13487 2023-11-27 14:22:26.067260 openshift_python_utilities-5.0.9/ocp_utilities/infra.py
+-rw-r--r--   0        0        0     8016 2023-11-27 14:22:26.067260 openshift_python_utilities-5.0.9/ocp_utilities/monitoring.py
+-rw-r--r--   0        0        0     1877 2023-11-27 14:22:26.067260 openshift_python_utilities-5.0.9/ocp_utilities/must_gather.py
+-rw-r--r--   0        0        0    14087 2023-11-27 14:22:26.067260 openshift_python_utilities-5.0.9/ocp_utilities/operators.py
+-rw-r--r--   0        0        0     3441 2023-11-27 14:22:26.067260 openshift_python_utilities-5.0.9/ocp_utilities/utils.py
+-rw-r--r--   0        0        0     1546 2023-11-27 14:22:30.801218 openshift_python_utilities-5.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 openshift_python_utilities-5.0.9/PKG-INFO
```

### Comparing `openshift_python_utilities-5.0.8/LICENSE` & `openshift_python_utilities-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_python_utilities-5.0.8/README.md` & `openshift_python_utilities-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openshift_python_utilities-5.0.8/ocp_utilities/infra.py` & `openshift_python_utilities-5.0.9/ocp_utilities/infra.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,20 @@
     LOGGER.info("Verify all pods are not failed nor pending.")
 
     failed_or_pending_pods = []
     for pod in pods:
         if pod.exists:
             pod_status = pod.instance.status.phase
             if pod_status in [pod.Status.PENDING, pod.Status.FAILED]:
-                failed_or_pending_pods.append(
-                    f"name: {pod.name}, namespace: {pod.namespace}, status:" f" {pod_status}\n"
-                )
+                failed_or_pending_pods.append(f"name: {pod.name}, namespace: {pod.namespace}, status: {pod_status}\n")
 
     if failed_or_pending_pods:
         failed_or_pending_pods_str = "\t".join(map(str, failed_or_pending_pods))
         raise PodsFailedOrPendingError(
-            "The following pods are failed or" f" pending:\n\t{failed_or_pending_pods_str}",
+            f"The following pods are failed or pending:\n\t{failed_or_pending_pods_str}",
         )
 
 
 def assert_nodes_in_healthy_condition(
     nodes,
     healthy_node_condition_type=None,
 ):
@@ -183,15 +181,15 @@
 
     if unhealthy_nodes_with_conditions:
         nodes_unhealthy_condition_error_str = json.dumps(
             unhealthy_nodes_with_conditions,
             indent=3,
         )
         raise NodesNotHealthyConditionError(
-            "Following are nodes with unhealthy" f" condition/s:\n{nodes_unhealthy_condition_error_str}"
+            f"Following are nodes with unhealthy condition/s:\n{nodes_unhealthy_condition_error_str}"
         )
 
 
 class DynamicClassCreator:
     """
     Taken from https://stackoverflow.com/a/66815839
     """
@@ -224,15 +222,15 @@
                     if data_collector_dict:
                         data_collector_directory = get_data_collector_base_dir(data_collector_dict=data_collector_dict)
 
                         collect_data_function = data_collector_dict["collect_data_function"]
                         module_name, function_name = collect_data_function.rsplit(".", 1)
                         import_module = importlib.import_module(name=module_name)
                         collect_data_function = getattr(import_module, function_name)
-                        LOGGER.info("[Data collector] Collecting data for" f" {self.kind} {self.name}")
+                        LOGGER.info(f"[Data collector] Collecting data for {self.kind} {self.name}")
                         collect_data_function(
                             directory=data_collector_directory,
                             resource_object=self,
                             collect_pod_logs=data_collector_dict.get("collect_pod_logs", False),
                         )
                 except Exception as exception_:
                     LOGGER.warning(
@@ -290,15 +288,15 @@
         pull_secret (str): Path to your registry credentials, default set to None(until passed)
         filter_options (str): when filter passed it will choose image from multiple variants.
 
     Returns:
         str: base command to create icsp in the cluster.
     """
     base_command = (
-        f"oc adm catalog mirror {image} {source_url} --manifests-only " f"--to-manifests {folder_name} {filter_options}"
+        f"oc adm catalog mirror {image} {source_url} --manifests-only --to-manifests {folder_name} {filter_options}"
     )
     if pull_secret:
         base_command = f"{base_command} --registry-config={pull_secret}"
     return base_command
 
 
 def generate_icsp_file(folder_name, image, source_url, pull_secret=None, filter_options=""):
```

### Comparing `openshift_python_utilities-5.0.8/ocp_utilities/monitoring.py` & `openshift_python_utilities-5.0.9/ocp_utilities/monitoring.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,41 +33,50 @@
 
     def __init__(
         self,
         namespace="openshift-monitoring",
         resource_name="prometheus-k8s",
         client=None,
         verify_ssl=True,
+        bearer_token=None,
     ):
+        """
+        Args:
+            namespace (str): Prometheus API resource namespace
+            resource_name (str): Prometheus API resource name
+            client (DynamicClient): Admin client resource
+            verify_ssl (bool): Perform SSL verification on query
+            bearer_token (str): Used for query OAuth with API endpoint
+        """
         self.namespace = namespace
         self.resource_name = resource_name
         self.client = client or get_client()
         self.api_v1 = "/api/v1"
         self.verify_ssl = verify_ssl
+        self.bearer_token = bearer_token
         self.api_url = self._get_route()
         self.headers = self._get_headers()
         self.scrape_interval = self.get_scrape_interval()
 
     def _get_route(self):
         # get route to prometheus HTTP api
         LOGGER.info("Prometheus: Obtaining route")
         route = Route(namespace=self.namespace, name=self.resource_name, client=self.client).instance.spec.host
 
         return f"https://{route}"
 
     def _get_headers(self):
-        """Uses the Prometheus serviceaccount to get an access token for OAuth"""
-
+        """Uses the Prometheus serviceaccount to get an access token for OAuth if not given"""
         LOGGER.info("Setting Prometheus headers and Obtaining OAuth token")
 
-        secret = self._get_resource_secret()
-
-        token = secret.instance.metadata.annotations["openshift.io/token-secret.value"]
+        if not self.bearer_token:
+            secret = self._get_resource_secret()
+            self.bearer_token = secret.instance.metadata.annotations["openshift.io/token-secret.value"]
 
-        return {"Authorization": f"Bearer {token}"}
+        return {"Authorization": f"Bearer {self.bearer_token}"}
 
     def _get_service_account(self):
         """get service account  for the given namespace and resource"""
 
         return ServiceAccount(namespace=self.namespace, name=self.resource_name, client=self.client)
 
     def _get_resource_secret(self):
@@ -149,15 +158,15 @@
         """
         get prometheus scrap interval
 
         Returns:
              int: scrape time interval or default 30 if not found
         """
         response = self._get_response(query=f"{self.api_v1}/targets")
-        result = response["data"]["activeTargets"]
+        result = response.get("data", {}).get("activeTargets", [])
         for item in result:
             if item and item["labels"]["job"] == "prometheus-k8s":
                 scrape_interval = item["scrapeInterval"]
                 return int((re.match(r"\d+", scrape_interval)).group())
         return 30
 
     def query_sampler(self, query, timeout=TIMEOUT_2MIN):
@@ -182,15 +191,15 @@
         )
         sample = None
         try:
             for sample in sampler:
                 if sample["status"] == "success":
                     return sample.get("data", {}).get("result")
         except TimeoutExpiredError:
-            LOGGER.error(f"Failed to get successful status after executing query '{query}'." f" Query result: {sample}")
+            LOGGER.error(f"Failed to get successful status after executing query '{query}'. Query result: {sample}")
             raise
 
     def alerts(self):
         """
         get all the active alerts
         """
         return self._get_response(query=f"{self.api_v1}/alerts")
```

### Comparing `openshift_python_utilities-5.0.8/ocp_utilities/must_gather.py` & `openshift_python_utilities-5.0.9/ocp_utilities/must_gather.py`

 * *Files identical despite different names*

### Comparing `openshift_python_utilities-5.0.8/ocp_utilities/operators.py` & `openshift_python_utilities-5.0.9/ocp_utilities/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 return cluster_resource(InstallPlan)(
                     client=admin_client,
                     name=install_plan["name"],
                     namespace=subscription.namespace,
                 )
     except TimeoutExpiredError:
         LOGGER.error(
-            f"Subscription: {subscription.name}, did not get updated with install plan:" f" {pformat(subscription)}"
+            f"Subscription: {subscription.name}, did not get updated with install plan: {pformat(subscription)}"
         )
         raise
 
 
 def wait_for_operator_install(admin_client, subscription, timeout=TIMEOUT_5MIN):
     """
     Wait for the operator to be installed, including InstallPlan and CSV ready.
```

### Comparing `openshift_python_utilities-5.0.8/ocp_utilities/utils.py` & `openshift_python_utilities-5.0.9/ocp_utilities/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         timeout=timeout,
         **kwargs,
     )
     out_decoded = sub_process.stdout
     err_decoded = sub_process.stderr
 
     error_msg = (
-        f"Failed to run {command_for_log}. rc: {sub_process.returncode}, out:" f" {out_decoded}, error: {err_decoded}"
+        f"Failed to run {command_for_log}. rc: {sub_process.returncode}, out: {out_decoded}, error: {err_decoded}"
     )
 
     if sub_process.returncode != 0:
         LOGGER.error(error_msg)
         return False, out_decoded, err_decoded
 
     # From this point and onwards we are guaranteed that sub_process.returncode == 0
```

### Comparing `openshift_python_utilities-5.0.8/pyproject.toml` & `openshift_python_utilities-5.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "openshift-python-utilities"
-version = "5.0.8"
+version = "5.0.9"
 description = "A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper"
 authors = ["Meni Yakove <myakove@gmail.com>", "Ruth Netser <rnetser@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "ocp_utilities"}]
 homepage = "https://github.com/RedHatQE/openshift-python-utilities"
 documentation = "https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md"
```

### Comparing `openshift_python_utilities-5.0.8/PKG-INFO` & `openshift_python_utilities-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 5.0.8
+Version: 5.0.9
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Home-page: https://github.com/RedHatQE/openshift-python-utilities
 License: Apache-2.0
 Keywords: Openshift,ocp
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
```

