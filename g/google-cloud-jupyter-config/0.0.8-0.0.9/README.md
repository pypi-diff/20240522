# Comparing `tmp/google_cloud_jupyter_config-0.0.8.tar.gz` & `tmp/google_cloud_jupyter_config-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_cloud_jupyter_config-0.0.8.tar", last modified: Thu May  2 17:05:52 2024, max compression
+gzip compressed data, was "google_cloud_jupyter_config-0.0.9.tar", last modified: Wed May 22 01:31:45 2024, max compression
```

## Comparing `google_cloud_jupyter_config-0.0.8.tar` & `google_cloud_jupyter_config-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.341249 google_cloud_jupyter_config-0.0.8/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)    11358 2023-08-11 16:50:41.000000 google_cloud_jupyter_config-0.0.8/LICENSE
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       15 2023-08-11 16:50:41.000000 google_cloud_jupyter_config-0.0.8/MANIFEST.in
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-05-02 17:05:52.340249 google_cloud_jupyter_config-0.0.8/PKG-INFO
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1682 2023-08-11 16:50:41.000000 google_cloud_jupyter_config-0.0.8/README.md
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.337249 google_cloud_jupyter_config-0.0.8/google/
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.338249 google_cloud_jupyter_config-0.0.8/google/cloud/
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.340249 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      830 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/__init__.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     5387 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2588 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config_test.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2909 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/tokenrenewer.py
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.340249 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/PKG-INFO
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      467 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/SOURCES.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)        1 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/dependency_links.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       43 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/requires.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       12 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/top_level.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       67 2024-05-02 17:05:52.341249 google_cloud_jupyter_config-0.0.8/setup.cfg
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1254 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/setup.py
+drwxr-x---   0 ojarjur  (106486) primarygroup (89939)        0 2024-05-22 01:31:45.477028 google_cloud_jupyter_config-0.0.9/
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)    11358 2023-10-06 19:02:49.000000 google_cloud_jupyter_config-0.0.9/LICENSE
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)       15 2023-10-06 19:02:49.000000 google_cloud_jupyter_config-0.0.9/MANIFEST.in
+-rw-r--r--   0 ojarjur  (106486) primarygroup (89939)     2139 2024-05-22 01:31:45.477028 google_cloud_jupyter_config-0.0.9/PKG-INFO
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)     1682 2023-10-06 19:02:49.000000 google_cloud_jupyter_config-0.0.9/README.md
+drwxr-x---   0 ojarjur  (106486) primarygroup (89939)        0 2024-05-22 01:31:45.473028 google_cloud_jupyter_config-0.0.9/google/
+drwxr-x---   0 ojarjur  (106486) primarygroup (89939)        0 2024-05-22 01:31:45.473028 google_cloud_jupyter_config-0.0.9/google/cloud/
+drwxr-x---   0 ojarjur  (106486) primarygroup (89939)        0 2024-05-22 01:31:45.477028 google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)      901 2024-05-22 01:31:02.000000 google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/__init__.py
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)     7678 2024-05-22 01:31:02.000000 google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/config.py
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)     2877 2024-05-22 01:31:02.000000 google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/config_test.py
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)     2909 2024-05-01 23:07:28.000000 google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/tokenrenewer.py
+drwxr-x---   0 ojarjur  (106486) primarygroup (89939)        0 2024-05-22 01:31:45.477028 google_cloud_jupyter_config-0.0.9/google_cloud_jupyter_config.egg-info/
+-rw-r--r--   0 ojarjur  (106486) primarygroup (89939)     2139 2024-05-22 01:31:45.000000 google_cloud_jupyter_config-0.0.9/google_cloud_jupyter_config.egg-info/PKG-INFO
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)      467 2024-05-22 01:31:45.000000 google_cloud_jupyter_config-0.0.9/google_cloud_jupyter_config.egg-info/SOURCES.txt
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)        1 2024-05-22 01:31:45.000000 google_cloud_jupyter_config-0.0.9/google_cloud_jupyter_config.egg-info/dependency_links.txt
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)       43 2024-05-22 01:31:45.000000 google_cloud_jupyter_config-0.0.9/google_cloud_jupyter_config.egg-info/requires.txt
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)       12 2024-05-22 01:31:45.000000 google_cloud_jupyter_config-0.0.9/google_cloud_jupyter_config.egg-info/top_level.txt
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)       67 2024-05-22 01:31:45.477028 google_cloud_jupyter_config-0.0.9/setup.cfg
+-rw-r-----   0 ojarjur  (106486) primarygroup (89939)     1307 2024-05-22 01:31:02.000000 google_cloud_jupyter_config-0.0.9/setup.py
```

### Comparing `google_cloud_jupyter_config-0.0.8/LICENSE` & `google_cloud_jupyter_config-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.8/PKG-INFO` & `google_cloud_jupyter_config-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-jupyter-config
-Version: 0.0.8
+Version: 0.0.9
 Summary: Jupyter configuration utilities using gcloud
 Home-page: https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config
 Author: Google, Inc.
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google_cloud_jupyter_config-0.0.8/README.md` & `google_cloud_jupyter_config-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/__init__.py` & `google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from google.cloud.jupyter_config.config import async_get_gcloud_config
 from google.cloud.jupyter_config.config import get_gcloud_config
 from google.cloud.jupyter_config.config import gcp_project
 from google.cloud.jupyter_config.config import gcp_region
 from google.cloud.jupyter_config.config import configure_gateway_client
```

### Comparing `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config.py` & `google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import asyncio
 import datetime
 import json
 import subprocess
 import sys
 import tempfile
 
 import cachetools
@@ -44,24 +45,56 @@
             encoding="UTF-8",
             shell=True,
         )
         t.seek(0)
         return t.read().decode("UTF-8").strip()
 
 
+async def async_run_gcloud_subcommand(subcmd):
+    """Run a specified gcloud sub-command and return its output.
+
+    The supplied subcommand is the full command line invocation, *except* for
+    the leading `gcloud` being omitted.
+
+    e.g. `info` instead of `gcloud info`.
+
+    We reuse the system stderr for the command so that any prompts from gcloud
+    will be displayed to the user.
+    """
+    with tempfile.TemporaryFile() as t:
+        p = await asyncio.create_subprocess_shell(
+            f"gcloud {subcmd}",
+            stdin=subprocess.DEVNULL,
+            stderr=sys.stderr,
+            stdout=t,
+            check=True,
+        )
+        await p.wait()
+        t.seek(0)
+        return t.read().decode("UTF-8").strip()
+
+
 @cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=(20 * 60)))
 def cached_gcloud_subcommand(subcmd):
     return run_gcloud_subcommand(subcmd)
 
 
 def clear_gcloud_cache():
     """Clear the TTL cache used to cache gcloud subcommand results."""
     cached_gcloud_subcommand.cache_clear()
 
 
+def _get_config_field(config, field):
+    subconfig = config
+    for path_part in field.split("."):
+        if path_part:
+            subconfig = subconfig.get(path_part, {})
+    return subconfig
+
+
 def get_gcloud_config(field):
     """Helper method that invokes the gcloud config helper.
 
     Invoking gcloud commands is a very heavyweight process, so the config is
     cached for up to 20 minutes.
 
     The config is generated with a minimum credential expiry of 30 minutes, so
@@ -79,21 +112,47 @@
         then the return value will be a string. In comparison, if the field
         is `configuration.properties.core`, then the return value will be a
         dictionary containing a field named `project` with a string value.
     """
     subcommand = "config config-helper --min-expiry=30m --format=json"
     cached_config_str = cached_gcloud_subcommand(subcommand)
     cached_config = json.loads(cached_config_str)
+    return _get_config_field(cached_config, field)
 
-    subconfig = cached_config
-    for path_part in field.split("."):
-        if path_part:
-            subconfig = subconfig.get(path_part, {})
 
-    return subconfig
+async def async_get_gcloud_config(field):
+    """Async helper method that invokes the gcloud config helper.
+
+    This is like `get_gcloud_config` but does not block on the underlying
+    gcloud invocation when there is a cache miss.
+
+    Args:
+        field: A period-separated search path for the config value to return.
+               For example, 'configuration.properties.core.project'
+    Returns:
+        An awaitable that resolves to a JSON object with a type depending on
+        the search path for the field within the gcloud config.
+
+        For example, if the field is `configuration.properties.core.project`,
+        then the JSON object will be a string. In comparison, if the field
+        is `configuration.properties.core`, then it will be a dictionary
+        containing a field named `project` with a string value.
+    """
+    subcommand = "config config-helper --min-expiry=30m --format=json"
+    with cached_gcloud_subcommand.cache_lock:
+        if subcommand in cached_gcloud_subcommand.cache:
+            cached_config_str = cached_gcloud_subcommand.cache[subcommand]
+            cached_config = json.loads(cached_config_str)
+            return _get_config_field(cached_config, field)
+
+    out = await async_run_gcloud_subcommand(subcommand)
+    with cached_gcloud_subcommand.cache_lock:
+        cached_gcloud_subcommand.cache[subcommand] = out
+    config = json.loads(cached_config_str)
+    return _get_config_field(config, field)
 
 
 def gcp_account():
     """Helper method to get the project configured through gcloud"""
     return get_gcloud_config("configuration.properties.core.account")
```

### Comparing `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config_test.py` & `google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/config_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import unittest
 
 from google.cloud.jupyter_config.config import (
+    async_get_gcloud_config,
     gcp_account,
     gcp_credentials,
     gcp_project,
     gcp_region,
     clear_gcloud_cache,
 )
+import pytest
 
 
 class TestConfig(unittest.TestCase):
     _mock_cloudsdk_variables = {
         "CLOUDSDK_AUTH_ACCESS_TOKEN": "example-token",
         "CLOUDSDK_CORE_ACCOUNT": "example-account",
         "CLOUDSDK_CORE_PROJECT": "example-project",
@@ -64,10 +66,17 @@
         self.assertEqual(gcp_project(), "example-project")
 
     def test_gcp_region(self):
         self.assertEqual(gcp_region(), "example-region")
         os.environ["CLOUDSDK_DATAPROC_REGION"] = "should-not-be-used"
         self.assertEqual(gcp_region(), "example-region")
 
+    @pytest.mark.asyncio
+    async def test_async_gcloud_config(self):
+        test_account = await async_get_gcloud_config(
+            "configuration.properties.core.account"
+        )
+        self.assertEqual(test_account, "example-account")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/tokenrenewer.py` & `google_cloud_jupyter_config-0.0.9/google/cloud/jupyter_config/tokenrenewer.py`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/PKG-INFO` & `google_cloud_jupyter_config-0.0.9/google_cloud_jupyter_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-jupyter-config
-Version: 0.0.8
+Version: 0.0.9
 Summary: Jupyter configuration utilities using gcloud
 Home-page: https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config
 Author: Google, Inc.
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google_cloud_jupyter_config-0.0.8/setup.py` & `google_cloud_jupyter_config-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="google-cloud-jupyter-config",
     author="Google, Inc.",
-    version="0.0.8",
+    version="0.0.9",
     description="Jupyter configuration utilities using gcloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config",
     license="Apache License 2.0",
     packages=setuptools.find_namespace_packages(),
     python_requires=">=3.8",
     install_requires=[
         "cachetools",
         "jupyter_server>=2.4.0",
         "traitlets",
     ],
+    tests_require=[
+        "pytest-asyncio",
+    ],
 )
```

