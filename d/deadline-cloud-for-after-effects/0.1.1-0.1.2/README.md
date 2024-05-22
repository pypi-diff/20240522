# Comparing `tmp/deadline_cloud_for_after_effects-0.1.1.tar.gz` & `tmp/deadline_cloud_for_after_effects-0.1.2.tar.gz`

## Comparing `deadline_cloud_for_after_effects-0.1.1.tar` & `deadline_cloud_for_after_effects-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,45 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/_version.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/hatch_custom_hook.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/_version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/AEAdaptor.json
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/__init__.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/__main__.py
--rw-r--r--   0        0        0    15763 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/py.typed
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/__init__.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_client.py
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_handler.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ipc.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/NOTICE
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/hatch.toml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/_version.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/hatch_custom_hook.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/_version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/AEAdaptor.json
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/__init__.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/__main__.py
+-rw-r--r--   0        0        0    15763 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/py.typed
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEClient/__init__.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEClient/ae_client.py
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEClient/ae_handler.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEClient/ipc.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/DeadlineVersionRequirement.jsx
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/Imports.jsx
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/OpenAESubmitter.jsx
+-rw-r--r--   0        0        0   107153 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/UI/AESubmitterUI.jsx
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/UI/CloseButton.jsx
+-rw-r--r--   0        0        0    34793 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/UI/SettingsWindow.jsx
+-rw-r--r--   0        0        0    31347 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/UI/SubmitButton.jsx
+-rw-r--r--   0        0        0    34943 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/UI/SubmitLayersWindow.jsx
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/ae_templates/parameter_values.json
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/ae_templates/template.json
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/data/DeadlineData.jsx
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/data/InitData.jsx
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/data/Property.jsx
+-rw-r--r--   0        0        0    46809 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/polyfill/index.js
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/submission/AssetReferenceTemplate.jsx
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/submission/DataTemplate.jsx
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/submission/JobTemplate.jsx
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/submission/SubmitBundle.jsx
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/utils/AeUtil.jsx
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/utils/DeadlineCommands.jsx
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/utils/Logger.jsx
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/utils/Settings.jsx
+-rw-r--r--   0        0        0    37087 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_submitter/utils/Util.jsx
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/NOTICE
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/hatch.toml
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.2/PKG-INFO
```

### Comparing `deadline_cloud_for_after_effects-0.1.1/hatch_custom_hook.py` & `deadline_cloud_for_after_effects-0.1.2/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/__main__.py` & `deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/adaptor.py` & `deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_client.py` & `deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEClient/ae_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_handler.py` & `deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEClient/ae_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ipc.py` & `deadline_cloud_for_after_effects-0.1.2/src/deadline/ae_adaptor/AEClient/ipc.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/LICENSE` & `deadline_cloud_for_after_effects-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/README.md` & `deadline_cloud_for_after_effects-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/hatch.toml` & `deadline_cloud_for_after_effects-0.1.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.1/pyproject.toml` & `deadline_cloud_for_after_effects-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -62,18 +62,18 @@
 
 [tool.hatch.build.hooks.custom.copy_version_py]
 destinations = [
   "src/deadline/ae_adaptor"
 ]
 
 [tool.hatch.build.targets.sdist]
-include = ["src/deadline/ae_adaptor/*", "hatch_custom_hook.py"]
+include = ["src/deadline/*", "hatch_custom_hook.py"]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/deadline/ae_adaptor"]
+packages = ["src/deadline"]
 
 # --- MYPY ---
 
 [tool.mypy]
 python_version = "3.9"
 check_untyped_defs = true
 show_error_codes = true
```

### Comparing `deadline_cloud_for_after_effects-0.1.1/PKG-INFO` & `deadline_cloud_for_after_effects-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-after-effects
-Version: 0.1.1
+Version: 0.1.2
 Summary: AWS Deadline Cloud for After Effects
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-after-effects
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-after-effects
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

