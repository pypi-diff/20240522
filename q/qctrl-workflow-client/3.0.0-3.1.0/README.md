# Comparing `tmp/qctrl_workflow_client-3.0.0.tar.gz` & `tmp/qctrl_workflow_client-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_workflow_client-3.0.0.tar", max compression
+gzip compressed data, was "qctrl_workflow_client-3.1.0.tar", max compression
```

## Comparing `qctrl_workflow_client-3.0.0.tar` & `qctrl_workflow_client-3.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    36587 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/LICENSE
--rw-r--r--   0        0        0      223 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/README.md
--rw-r--r--   0        0        0     2785 2024-03-18 01:36:21.162312 qctrl_workflow_client-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      954 2024-03-18 01:36:21.170313 qctrl_workflow_client-3.0.0/qctrlworkflowclient/__init__.py
--rw-r--r--   0        0        0     3311 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/defaults.py
--rw-r--r--   0        0        0     2642 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/functions.py
--rw-r--r--   0        0        0     1583 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/globals.py
--rw-r--r--   0        0        0      969 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/products.py
--rw-r--r--   0        0        0      638 2024-03-18 01:36:21.174313 qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/__init__.py
--rw-r--r--   0        0        0    23574 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/api.py
--rw-r--r--   0        0        0     1206 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/base.py
--rw-r--r--   0        0        0     1201 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/local.py
--rw-r--r--   0        0        0     3332 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/settings.py
--rw-r--r--   0        0        0     5361 2024-03-18 01:35:55.900138 qctrl_workflow_client-3.0.0/qctrlworkflowclient/utils.py
--rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 qctrl_workflow_client-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-05-22 02:04:53.984077 qctrl_workflow_client-3.1.0/LICENSE
+-rw-r--r--   0        0        0      223 2024-05-22 02:04:53.984077 qctrl_workflow_client-3.1.0/README.md
+-rw-r--r--   0        0        0     2785 2024-05-22 02:05:17.628090 qctrl_workflow_client-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      954 2024-05-22 02:05:17.632090 qctrl_workflow_client-3.1.0/qctrlworkflowclient/__init__.py
+-rw-r--r--   0        0        0     3311 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/defaults.py
+-rw-r--r--   0        0        0     4840 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/functions.py
+-rw-r--r--   0        0        0     1583 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/globals.py
+-rw-r--r--   0        0        0      969 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/products.py
+-rw-r--r--   0        0        0      638 2024-05-22 02:05:17.636090 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/__init__.py
+-rw-r--r--   0        0        0    24063 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/api.py
+-rw-r--r--   0        0        0     1206 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/base.py
+-rw-r--r--   0        0        0     1201 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/local.py
+-rw-r--r--   0        0        0     3332 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/settings.py
+-rw-r--r--   0        0        0     5361 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/utils.py
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 qctrl_workflow_client-3.1.0/PKG-INFO
```

### Comparing `qctrl_workflow_client-3.0.0/LICENSE` & `qctrl_workflow_client-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/pyproject.toml` & `qctrl_workflow_client-3.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-workflow-client"
-version = "3.0.0"
+version = "3.1.0"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com"
@@ -75,21 +75,21 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 tomli = "^2.0.1"
 importlib-metadata = "^6.8.0"
 gql = "^3.4.0"
 tenacity = "^8.1.0"
-requests = "^2.31.0"
+requests = "^2.32.0"
 packaging = "^23.1.0"
 qctrl-commons = { version = "^22.0.0", source = "PyPI" }
 qctrl-client = { version = "^9.1.0", source = "PyPI" }
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
+black = "^24.3.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.3"
 pylint = "^2.14.4"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
```

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/__init__.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 from .defaults import (
     get_authenticated_client_for_product,
     get_default_api_url,
     get_default_cli_auth,
     get_default_oidc_url,
 )
```

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/defaults.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/functions.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/functions.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     Any,
     Callable,
     Dict,
     Optional,
 )
 from warnings import warn
 
+from qctrlcommons.exceptions import QctrlArgumentsValueError
+
 
 def core_workflow(
     get_config: Callable, workflow: str, formatter: Optional[Callable] = None
 ):
     """
     Decorator for a function which will execute a workflow.
     The decorated function should return the data to be used
@@ -57,14 +59,79 @@
         @wraps(func)
         def customized_decorator(*args, **kwargs):
             # router is instantiated before function is called
             # so any alteration to settings is visible within
             # the function
             config = get_config()
             router = config.get_router()
+
+            router.set_async_state(kwargs.pop("is_async", False))
+
+            data = func(*args, **kwargs)
+            result = router(workflow, data)
+
+            if formatter:
+                result = formatter(result)
+
+            return result
+
+        return customized_decorator
+
+    return decorator
+
+
+def async_core_workflow(
+    get_config: Callable, workflow: str, formatter: Optional[Callable] = None
+):
+    """
+    Decorator for a function which will execute asynchronously workflow.
+    The decorated function should return the data to be used
+    during async workflow execution. When being used in a client
+    package, it is recommended to use a partial to provide
+    a default value for `get_config` e.g.
+
+    async_fire_opal_workflow = partial(
+        async_core_workflow,
+        get_fire_opal_config
+    )
+
+    @async_fire_opal_workflow("execute")
+    def execute(...):
+
+    Parameters
+    ----------
+    get_config : Callable
+        Returns a `CoreClientSettings` instance. The configured
+        router will be used to execute the workflow.
+    workflow : str
+        The registered name of the workflow to be executed.
+    formatter : Callable, optional
+        Optional callable which can be used to format the workflow
+        result. The callable should accept exactly one argument
+        which is the raw result fo the workflow. If used, the
+        decorated function will return the result of this callable.
+    """
+
+    def decorator(func: Callable):
+        @wraps(func)
+        def customized_decorator(*args, **kwargs):
+            # router is instantiated before function is called
+            # so any alteration to settings is visible within
+            # the function
+            config = get_config()
+            router = config.get_router()
+
+            # Set the async state to True
+            router.set_async_state(True)
+            if "is_async" in kwargs:
+                raise QctrlArgumentsValueError(
+                    description="The asynchronous state of this function cannot be altered.",
+                    arguments={"is_async": kwargs.get("is_async")},
+                )
+
             data = func(*args, **kwargs)
             result = router(workflow, data)
 
             if formatter:
                 result = formatter(result)
 
             return result
```

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/globals.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/products.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/products.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/__init__.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/api.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,21 @@
     ]
 
     def __init__(self, client: GraphQLClient, settings: CoreClientSettings):
         self._client = client
         self._settings = settings
         self._validate()
         self._parallel_task_collector = None
+        self._async = False
+
+    def set_async_state(self, is_async: bool):
+        """
+        Toggle asynchronous state of workflow execution.
+        """
+        self._async = is_async
 
     def _validate(self):
         """
         Perform validation checks on the settings.
         """
 
         if not self._settings.product:
@@ -380,14 +387,17 @@
         action = Action(
             action_id=action_data["modelId"],
             status=action_data["status"],
             raw_result=action_data["result"],
             errors=action_data["errors"],
         )
 
+        if self._async:
+            return {"async_result": action}
+
         if self._parallel_task_collector is not None:
             async_result = {"async_result": action}
             self._parallel_task_collector.add(async_result)
             return async_result
 
         return self.get_result(action)
 
@@ -424,24 +434,19 @@
         Handle warnings returned when starting a workflow.
         """
 
         for warning_data in warnings_data:
             message = warning_data["message"]
             warn(Warning(message))
 
-    @retry(
-        wait=_POLL_WAIT_CHAIN,
-        retry=retry_if_result(lambda action: not action.is_finished()),
-    )
-    def _poll_for_completion(self, action: Action) -> Action:
+    def update_action_status(self, action: Action) -> Action:
         """
-        Poll the API waiting for the action to be finished.
-        When finished, an updated `Action` object is returned.
+        Update the action status. When finished, an updated
+        `Action` object is returned.
         """
-
         _query = gql.gql(
             """
             query($modelId: String!) {
                 action(modelId: $modelId) {
                     action {
                         status
                         errors {
@@ -463,14 +468,25 @@
         action.raw_result = response["action"]["action"]["result"]
         action.errors = response["action"]["action"]["errors"]
 
         self._settings.event_dispatch("action.updated", action=action)
 
         return action
 
+    @retry(
+        wait=_POLL_WAIT_CHAIN,
+        retry=retry_if_result(lambda action: not action.is_finished()),
+    )
+    def _poll_for_completion(self, action: Action) -> Action:
+        """
+        Poll the API waiting for the action to be finished.
+        When finished, an updated `Action` object is returned.
+        """
+        return self.update_action_status(action)
+
     def get_result(self, action: Action) -> DecodedResult:
         """
         Return the result of the action.
         """
         return self._fetch_action(action).result
 
     def _fetch_action(self, action: Action) -> Any:
```

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/base.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/router/local.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/settings.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/qctrlworkflowclient/utils.py` & `qctrl_workflow_client-3.1.0/qctrlworkflowclient/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.0.0/PKG-INFO` & `qctrl_workflow_client-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-workflow-client
-Version: 3.0.0
+Version: 3.1.0
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -29,15 +29,15 @@
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
 Requires-Dist: packaging (>=23.1.0,<24.0.0)
 Requires-Dist: qctrl-client (>=9.1.0,<10.0.0)
 Requires-Dist: qctrl-commons (>=22.0.0,<23.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.0,<3.0.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
```

