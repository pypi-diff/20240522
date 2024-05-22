# Comparing `tmp/deadline_cloud_for_houdini-0.6.2.tar.gz` & `tmp/deadline_cloud_for_houdini-0.6.3.tar.gz`

## Comparing `deadline_cloud_for_houdini-0.6.2.tar` & `deadline_cloud_for_houdini-0.6.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/_version.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
--rw-r--r--   0        0        0    20824 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/_version.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
--rw-r--r--   0        0        0    23586 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_assets.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
--rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
--rw-r--r--   0        0        0    24481 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/NOTICE
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/hatch.toml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/_version.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
+-rw-r--r--   0        0        0    20824 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/_version.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
+-rw-r--r--   0        0        0    23586 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_assets.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
+-rw-r--r--   0        0        0    25079 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/NOTICE
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/hatch.toml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.3/PKG-INFO
```

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_assets.py` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_assets.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,19 @@
 
 
 def get_queue_parameter_definitions_from_service(farm_id: str, queue_id: str) -> list[JobParameter]:
     return get_queue_parameter_definitions(farmId=farm_id, queueId=queue_id)
 
 
 def update_queue_parameters(farm_id: str, queue_id: str, node: hou.Node) -> None:
+    """
+    :farm_id: a valid Deadline Cloud farm ID that the user has access to
+    :queue_id: a valid Deadline Cloud queue ID that the user has access to
+    :node: Deadline Cloud ROP node
+    """
     queue_parameter_definitions = get_queue_parameter_definitions_from_service(farm_id, queue_id)
     queue_parameter_definitions_json = json.dumps(queue_parameter_definitions)
     node.setUserData("queue_parameter_definitions", queue_parameter_definitions_json)
 
     # When we rebuild the UI, we want to keep any values for parameters
     # that the user has already entered.
     existing_values = _get_queue_parameter_values(node, queue_parameter_definitions)
```

### Comparing `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py` & `deadline_cloud_for_houdini-0.6.3/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     _IGNORE_REF_VALUES as IGNORE_REF_VALUES,  # noqa
 )
 from ._version import version
 
 import hou
 
 
+_NONE_SELECTED_TEXT = "<none selected>"
+_REFRESHING_TEXT = "<refreshing>"
+
+
 def _get_houdini_version() -> str:
     return hou.applicationVersionString()
 
 
 def _get_wedge_render_node(node: hou.Node):
     """Return ROP set as input or parameter to a wedge node
 
@@ -524,21 +528,37 @@
         # Initialize telemetry client, opt-out is respected
         api.get_deadline_cloud_library_telemetry_client().update_common_details(
             {
                 "deadline-cloud-for-houdini-submitter-version": version,
                 "houdini-version": _get_houdini_version(),
             }
         )
+        farm_id = get_setting("defaults.farm_id")
+        if not farm_id:
+            hou.ui.displayMessage(
+                "Please configure the farm ID in the AWS Deadline Cloud render node (ROP) settings",
+                title="Farm ID Required",
+                severity=hou.severityType.Warning,
+            )
+            return
+
+        queue_id = get_setting("defaults.queue_id")
+        if not queue_id:
+            hou.ui.displayMessage(
+                "Please configure the queue ID in the AWS Deadline Cloud render node (ROP) settings",
+                title="Queue ID Required",
+                severity=hou.severityType.Warning,
+            )
+            return
+
         deadline = api.get_boto3_client("deadline")
 
         job_bundle_dir = create_job_history_bundle_dir("houdini", name)
         _create_job_bundle(node, job_bundle_dir, asset_references)
 
-        farm_id = get_setting("defaults.farm_id")
-        queue_id = get_setting("defaults.queue_id")
         storage_profile_id = get_setting("settings.storage_profile_id")
 
         storage_profile = None
         if storage_profile_id:
             storage_profile = api.get_storage_profile_for_queue(
                 farm_id, queue_id, storage_profile_id, deadline
             )
@@ -575,53 +595,59 @@
         hou.ui.displayMessage(
             str(exc), title="Houdini Job Submission", severity=hou.severityType.Warning
         )
 
 
 def settings_callback(kwargs):
     node = kwargs["node"]
-    node.parm("farm").set("<refreshing>")
-    node.parm("queue").set("<refreshing>")
+    _show_farm_and_queue_as_refreshing(node)
     DeadlineConfigDialog.configure_settings(parent=hou.qt.mainWindow())
-    deadline = api.get_boto3_client("deadline")
-    farm_id = get_setting("defaults.farm_id")
-    farm_response = deadline.get_farm(farmId=farm_id)
-    node.parm("farm").set(farm_response["displayName"])
-    queue_id = get_setting("defaults.queue_id")
-    queue_response = deadline.get_queue(farmId=farm_id, queueId=queue_id)
-    node.parm("queue").set(queue_response["displayName"])
-    update_queue_parameters(farm_id, queue_id, node)
+    _apply_farm_and_queue_settings(node)
 
 
 def login_callback(kwargs):
     node = kwargs["node"]
-    node.parm("farm").set("<refreshing>")
-    node.parm("queue").set("<refreshing>")
+    _show_farm_and_queue_as_refreshing(node)
     DeadlineLoginDialog.login(parent=hou.qt.mainWindow())
-    deadline = api.get_boto3_client("deadline")
-    farm_id = get_setting("defaults.farm_id")
-    farm_response = deadline.get_farm(farmId=farm_id)
-    node.parm("farm").set(farm_response["displayName"])
-    queue_id = get_setting("defaults.queue_id")
-    queue_response = deadline.get_queue(farmId=farm_id, queueId=queue_id)
-    node.parm("queue").set(queue_response["displayName"])
-    update_queue_parameters(farm_id, queue_id, node)
+    _apply_farm_and_queue_settings(node)
 
 
 def logout_callback(kwargs):
     node = kwargs["node"]
-    node.parm("farm").set("")
-    node.parm("queue").set("")
+    node.parm("farm").set(_NONE_SELECTED_TEXT)
+    node.parm("queue").set(_NONE_SELECTED_TEXT)
     api.logout()
 
 
 def update_queue_parameters_callback(kwargs):
     node = kwargs["node"]
+    _show_farm_and_queue_as_refreshing(node)
+    _apply_farm_and_queue_settings(node)
+
+
+def _show_farm_and_queue_as_refreshing(node):
+    node.parm("farm").set(_REFRESHING_TEXT)
+    node.parm("queue").set(_REFRESHING_TEXT)
+
+
+def _apply_farm_and_queue_settings(node):
     farm_id = get_setting("defaults.farm_id")
+    if not farm_id:
+        node.parm("farm").set(_NONE_SELECTED_TEXT)
+        node.parm("queue").set(_NONE_SELECTED_TEXT)
+        return
+    deadline = api.get_boto3_client("deadline")
+    farm_response = deadline.get_farm(farmId=farm_id)
+    node.parm("farm").set(farm_response["displayName"])
     queue_id = get_setting("defaults.queue_id")
+    if not queue_id:
+        node.parm("queue").set(_NONE_SELECTED_TEXT)
+        return
+    queue_response = deadline.get_queue(farmId=farm_id, queueId=queue_id)
+    node.parm("queue").set(queue_response["displayName"])
     update_queue_parameters(farm_id, queue_id, node)
 
 
 # TODO: remove this and swap to default job template
 def get_houdini_environments(init_data_attachment: dict[str, Any]) -> list[dict[str, Any]]:
     """Returns a list of environments that set things up to run frame renders
     for the specified DCC.
```

### Comparing `deadline_cloud_for_houdini-0.6.2/LICENSE` & `deadline_cloud_for_houdini-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/README.md` & `deadline_cloud_for_houdini-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/hatch.toml` & `deadline_cloud_for_houdini-0.6.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.2/pyproject.toml` & `deadline_cloud_for_houdini-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 [tool.coverage.paths]
 source =  [
     "src/"
 ]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 48
+fail_under = 60
 
 [tool.semantic_release]
 # Can be removed or set to true once we are v1
 major_on_zero = false
 tag_format = "{version}"
 
 [tool.semantic_release.commit_parser_options]
```

### Comparing `deadline_cloud_for_houdini-0.6.2/PKG-INFO` & `deadline_cloud_for_houdini-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-houdini
-Version: 0.6.2
+Version: 0.6.3
 Summary: AWS Deadline Cloud for Houdini
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-houdini
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-houdini
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

