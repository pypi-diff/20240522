# Comparing `tmp/inferless_cli-1.1.7.tar.gz` & `tmp/inferless_cli-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless_cli-1.1.7.tar", max compression
+gzip compressed data, was "inferless_cli-1.1.8.tar", max compression
```

## Comparing `inferless_cli-1.1.7.tar` & `inferless_cli-1.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.7/README.md
--rw-r--r--   0        0        0       37 2024-05-21 06:49:34.982661 inferless_cli-1.1.7/inferless_cli/__init__.py
--rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.7/inferless_cli/__main__.py
--rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.7/inferless_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.7/inferless_cli/prompts/__init__.py
--rw-r--r--   0        0        0    23562 2024-05-21 06:49:34.982992 inferless_cli-1.1.7/inferless_cli/prompts/deploy.py
--rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.7/inferless_cli/prompts/export.py
--rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.7/inferless_cli/prompts/init.py
--rw-r--r--   0        0        0     3779 2024-04-30 07:21:43.512104 inferless_cli-1.1.7/inferless_cli/prompts/log.py
--rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.7/inferless_cli/prompts/login.py
--rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.7/inferless_cli/prompts/model.py
--rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.7/inferless_cli/prompts/run.py
--rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.7/inferless_cli/prompts/runtime.py
--rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.7/inferless_cli/prompts/secret.py
--rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.7/inferless_cli/prompts/token.py
--rw-r--r--   0        0        0    22378 2024-04-29 18:01:24.312203 inferless_cli-1.1.7/inferless_cli/prompts/volume.py
--rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.7/inferless_cli/prompts/workspace.py
--rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.7/inferless_cli/utils/__init__.py
--rw-r--r--   0        0        0     3492 2024-05-21 06:49:34.983395 inferless_cli-1.1.7/inferless_cli/utils/api.py
--rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.7/inferless_cli/utils/constants.py
--rw-r--r--   0        0        0     1277 2024-05-15 17:23:04.668037 inferless_cli-1.1.7/inferless_cli/utils/convertors.py
--rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.7/inferless_cli/utils/credentials.py
--rw-r--r--   0        0        0       48 2024-05-21 06:49:34.983775 inferless_cli-1.1.7/inferless_cli/utils/exceptions.py
--rw-r--r--   0        0        0    29299 2024-05-15 17:35:52.807108 inferless_cli-1.1.7/inferless_cli/utils/helpers.py
--rw-r--r--   0        0        0    27185 2024-05-21 06:49:34.984106 inferless_cli-1.1.7/inferless_cli/utils/services.py
--rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.7/inferless_cli/utils/validators.py
--rw-r--r--   0        0        0      671 2024-05-21 06:49:34.984814 inferless_cli-1.1.7/pyproject.toml
--rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.8/README.md
+-rw-r--r--   0        0        0       37 2024-05-22 06:58:56.263679 inferless_cli-1.1.8/inferless_cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.8/inferless_cli/__main__.py
+-rw-r--r--   0        0        0     7282 2024-05-22 06:10:40.237743 inferless_cli-1.1.8/inferless_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.8/inferless_cli/prompts/__init__.py
+-rw-r--r--   0        0        0    24025 2024-05-22 06:54:39.378644 inferless_cli-1.1.8/inferless_cli/prompts/deploy.py
+-rw-r--r--   0        0        0     1802 2024-05-22 06:10:40.242119 inferless_cli-1.1.8/inferless_cli/prompts/export.py
+-rw-r--r--   0        0        0    13104 2024-05-22 06:59:05.995069 inferless_cli-1.1.8/inferless_cli/prompts/init.py
+-rw-r--r--   0        0        0     3779 2024-05-22 06:10:40.245113 inferless_cli-1.1.8/inferless_cli/prompts/log.py
+-rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.8/inferless_cli/prompts/login.py
+-rw-r--r--   0        0        0    15846 2024-05-22 06:10:40.246662 inferless_cli-1.1.8/inferless_cli/prompts/model.py
+-rw-r--r--   0        0        0    18882 2024-05-22 06:10:40.247897 inferless_cli-1.1.8/inferless_cli/prompts/run.py
+-rw-r--r--   0        0        0     5984 2024-05-22 06:10:40.248956 inferless_cli-1.1.8/inferless_cli/prompts/runtime.py
+-rw-r--r--   0        0        0     2026 2024-05-22 06:10:40.249570 inferless_cli-1.1.8/inferless_cli/prompts/secret.py
+-rw-r--r--   0        0        0     4231 2024-05-22 06:10:40.250137 inferless_cli-1.1.8/inferless_cli/prompts/token.py
+-rw-r--r--   0        0        0    22378 2024-05-22 06:23:31.173738 inferless_cli-1.1.8/inferless_cli/prompts/volume.py
+-rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.8/inferless_cli/prompts/workspace.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.8/inferless_cli/utils/__init__.py
+-rw-r--r--   0        0        0     3492 2024-05-21 12:14:05.540759 inferless_cli-1.1.8/inferless_cli/utils/api.py
+-rw-r--r--   0        0        0    19491 2024-05-22 06:54:06.724477 inferless_cli-1.1.8/inferless_cli/utils/constants.py
+-rw-r--r--   0        0        0     1277 2024-05-22 06:10:40.253350 inferless_cli-1.1.8/inferless_cli/utils/convertors.py
+-rw-r--r--   0        0        0     7179 2024-05-22 06:10:40.256062 inferless_cli-1.1.8/inferless_cli/utils/credentials.py
+-rw-r--r--   0        0        0       48 2024-05-21 12:14:05.541168 inferless_cli-1.1.8/inferless_cli/utils/exceptions.py
+-rw-r--r--   0        0        0    29556 2024-05-22 06:35:37.344585 inferless_cli-1.1.8/inferless_cli/utils/helpers.py
+-rw-r--r--   0        0        0    27173 2024-05-22 06:58:47.680996 inferless_cli-1.1.8/inferless_cli/utils/services.py
+-rw-r--r--   0        0        0     7352 2024-05-22 06:21:04.479005 inferless_cli-1.1.8/inferless_cli/utils/validators.py
+-rw-r--r--   0        0        0      671 2024-05-22 06:59:15.601658 inferless_cli-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.8/PKG-INFO
```

### Comparing `inferless_cli-1.1.7/README.md` & `inferless_cli-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/main.py` & `inferless_cli-1.1.8/inferless_cli/main.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/deploy.py` & `inferless_cli-1.1.8/inferless_cli/prompts/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     validate_import_model,
     start_import_model,
     upload_file,
     validate_github_url_permissions,
     create_presigned_io_upload_url,
 )
 
-from inferless_cli.utils.constants import GITHUB, GIT
+from inferless_cli.utils.constants import GITHUB, GIT, REGION_MAP_KEYS
 
 
 def deploy_local(config_file_name, redeploy):
     is_yaml_present = is_inferless_yaml_present(config_file_name)
     old_response = None
     is_failed = False
     if is_yaml_present and not redeploy:
@@ -251,17 +251,22 @@
 
             status, res = poll_model_status(model_id)
             if status == "FAILURE":
                 error_msg = res["model_import"]["import_error"]["message"]
                 rich.print(f"[red]{error_msg}[/red]")
                 raise typer.Abort(1)
 
+            region = "region-2"
+            if "region" in config["configuration"]:
+                region = config["configuration"]["region"]
+
             default_values = get_default_machine_values(
                 config["configuration"]["gpu_type"],
                 "dedicated" if config["configuration"]["is_dedicated"] else "shared",
+                REGION_MAP_KEYS[region],
             )
 
             config_payload = {
                 "id": model_id,
                 "configuration": {
                     "runtime": "PYTORCH",
                     "cpu": float(default_values["cpu"]),
@@ -270,14 +275,15 @@
                     "is_dedicated": config["configuration"]["is_dedicated"],
                     "machine_type": config["configuration"]["gpu_type"],
                     "is_serverless": config["configuration"]["is_serverless"],
                     "max_replica": config["configuration"]["max_replica"],
                     "min_replica": config["configuration"]["min_replica"],
                     "memory": float(default_values["memory"]),
                     "scale_down_delay": config["configuration"]["scale_down_delay"],
+                    "region": region,
                 },
             }
 
             if (
                 config["configuration"]["custom_volume_id"]
                 and config["configuration"]["custom_volume_name"]
             ):
@@ -459,17 +465,22 @@
 
             status, res = poll_model_status(model_id)
             if status == "FAILURE":
                 error_msg = res["model_import"]["import_error"]["message"]
                 rich.print(f"[red]{error_msg}[/red]")
                 raise typer.Abort(1)
 
+            region = "region-2"
+            if "region" in config["configuration"]:
+                region = config["configuration"]["region"]
+
             default_values = get_default_machine_values(
                 config["configuration"]["gpu_type"],
                 "dedicated" if config["configuration"]["is_dedicated"] else "shared",
+                REGION_MAP_KEYS[region],
             )
 
             config_payload = {
                 "id": model_id,
                 "configuration": {
                     "runtime": "PYTORCH",
                     "cpu": float(default_values["cpu"]),
@@ -478,14 +489,15 @@
                     "is_dedicated": config["configuration"]["is_dedicated"],
                     "machine_type": config["configuration"]["gpu_type"],
                     "is_serverless": config["configuration"]["is_serverless"],
                     "max_replica": config["configuration"]["max_replica"],
                     "min_replica": config["configuration"]["min_replica"],
                     "memory": float(default_values["memory"]),
                     "scale_down_delay": config["configuration"]["scale_down_delay"],
+                    "region": region,
                 },
             }
 
             if (
                 config["configuration"]["custom_volume_id"]
                 and config["configuration"]["custom_volume_name"]
             ):
```

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/export.py` & `inferless_cli-1.1.8/inferless_cli/prompts/export.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/init.py` & `inferless_cli-1.1.8/inferless_cli/prompts/init.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import typer
 import rich
-from inferless_cli.utils.services import get_connected_accounts
+from inferless_cli.utils.services import get_connected_accounts, get_workspaces_list
 from inferless_cli.utils.helpers import (
     create_yaml,
+    decrypt_tokens,
+    get_machine_types_region_1,
     get_machine_types_serverless,
     get_machine_types_servers,
+    get_region_types,
     is_file_present,
     yaml,
     find_requirements_file,
     get_default_machine_values,
     get_frameworks,
     get_upload_methods,
     key_bindings,
@@ -18,16 +21,18 @@
     read_pyproject_toml,
     read_requirements_txt,
 )
 from inferless_cli.utils.validators import (
     has_github_provider,
     validate_framework,
     validate_machine_types,
+    validate_machine_types_region_1,
     validate_machine_types_server,
     validate_machine_types_serverless,
+    validate_region_types,
     validate_upload_method,
     validate_model_name,
     validate_url,
 )
 from inferless_cli.utils.constants import (
     DEFAULT_INFERLESS_RUNTIME_YAML_FILE,
     DEFAULT_INFERLESS_YAML_FILE,
@@ -39,14 +44,16 @@
     DEFAULT_INPUT_JSON,
     DEFAULT_OUTPUT_JSON,
     DEFAULT_INPUT_FILE_NAME,
     DEFAULT_OUTPUT_FILE_NAME,
     IO_DOCS_URL,
     MACHINE_TYPE_SERVERS_DEF,
     MACHINE_TYPES,
+    MACHINE_TYPES_REGION_1,
+    REGION_MAP_KEYS,
     RUNTIME_DOCS_URL,
     UPLOAD_METHODS,
 )
 from prompt_toolkit import prompt
 from prompt_toolkit.validation import Validator
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
@@ -151,22 +158,58 @@
             complete_while_typing=True,
             key_bindings=key_bindings,
             validator=Validator.from_callable(validate_machine_types_serverless),
             validate_while_typing=False,
         )
     else:
         deployment_type = "CONTAINER"
-        gpu_type = prompt(
-            f"GPU Type ({', '.join(str(x) for x in MACHINE_TYPES)}) : ",
-            completer=get_machine_types(),
-            complete_while_typing=True,
-            key_bindings=key_bindings,
-            validator=Validator.from_callable(validate_machine_types),
-            validate_while_typing=False,
-        )
+        try:
+            workspaces = get_workspaces_list()
+        except Exception as e:
+            rich.print(e)
+            raise typer.Exit(1)
+        _, _, _, workspace_id, _ = decrypt_tokens()
+        if name is None:
+            name = prompt(
+                "Enter the name for volume: ",
+            )
+        is_aws_enabled = False
+        for workspace in workspaces:
+            if workspace["id"] == workspace_id:
+                is_aws_enabled = workspace["is_aws_cluster_enabled"]
+                break
+
+        region = "region-2"
+        if is_aws_enabled:
+            region = prompt(
+                "Select Region ( region-1, region-2 ) : ",
+                completer=get_region_types(),
+                complete_while_typing=True,
+                key_bindings=key_bindings,
+                validator=Validator.from_callable(validate_region_types),
+                validate_while_typing=False,
+            )
+        if region == "region-2":
+            gpu_type = prompt(
+                f"GPU Type ({', '.join(str(x) for x in MACHINE_TYPES)}) : ",
+                completer=get_machine_types(),
+                complete_while_typing=True,
+                key_bindings=key_bindings,
+                validator=Validator.from_callable(validate_machine_types),
+                validate_while_typing=False,
+            )
+        elif region == "region-1":
+            gpu_type = prompt(
+                f"GPU Type ({', '.join(str(x) for x in MACHINE_TYPES_REGION_1)}) : ",
+                completer=get_machine_types_region_1(),
+                complete_while_typing=True,
+                key_bindings=key_bindings,
+                validator=Validator.from_callable(validate_machine_types_region_1),
+                validate_while_typing=False,
+            )
 
     is_dedicated = False
     is_custom_runtime = False
     if deployment_type == "CONTAINER":
         print_options("Server type:", MACHINE_TYPE_SERVERS_DEF)
         machine_type_server = prompt(
             "Do you want to use DEDICATED or SHARED server? ",
@@ -182,15 +225,15 @@
 
     if deployment_type == "SERVERLESS":
         is_dedicated = True
         config["configuration"]["is_dedicated"] = True
 
     # Get default values based on GPU Type and is_dedicated
     default_values = get_default_machine_values(
-        gpu_type, "dedicated" if is_dedicated else "shared"
+        gpu_type, "dedicated" if is_dedicated else "shared", REGION_MAP_KEYS[region]
     )
     requirements_file_name = None
     if is_custom_runtime:
         file_name_full, file_type, file_name = find_requirements_file()
         if file_name_full:
             # File is found
             rich.print(f"\nRequirements file found: {file_name}")
@@ -249,15 +292,15 @@
         rich.print("No dependencies specified or loaded.")
 
     # Prompts for non-serverless options
     # if deployment_type == "CONTAINER":
     config["configuration"]["custom_runtime_id"] = ""
     config["configuration"]["custom_volume_name"] = ""
     config["configuration"]["custom_volume_id"] = ""
-
+    config["configuration"]["region"] = region
     config["configuration"]["min_replica"] = "0"
     config["configuration"]["max_replica"] = "1"
     config["configuration"]["scale_down_delay"] = "600"
     config["optional"]["input_file_name"] = input_file_name
     config["optional"]["output_file_name"] = output_file_name
     config["configuration"]["inference_time"] = "180"
     if deployment_type == "CONTAINER":
```

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/log.py` & `inferless_cli-1.1.8/inferless_cli/prompts/log.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/login.py` & `inferless_cli-1.1.8/inferless_cli/prompts/login.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/model.py` & `inferless_cli-1.1.8/inferless_cli/prompts/model.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/run.py` & `inferless_cli-1.1.8/inferless_cli/prompts/run.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/runtime.py` & `inferless_cli-1.1.8/inferless_cli/prompts/runtime.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/secret.py` & `inferless_cli-1.1.8/inferless_cli/prompts/secret.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/token.py` & `inferless_cli-1.1.8/inferless_cli/prompts/token.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/volume.py` & `inferless_cli-1.1.8/inferless_cli/prompts/volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,23 +119,23 @@
         if workspace["id"] == workspace_id:
             is_aws_enabled = workspace["is_aws_cluster_enabled"]
             break
 
     region = None
     if is_aws_enabled:
         region = prompt(
-            "Select Region ( Region 1, Region 2 ) : ",
+            "Select Region ( region-1, region-2 ) : ",
             completer=get_region_types(),
             complete_while_typing=True,
             key_bindings=key_bindings,
             validator=Validator.from_callable(validate_region_types),
             validate_while_typing=False,
         )
     else:
-        region = "Region 2"
+        region = "region-2"
     res = None
     with Progress(
         SpinnerColumn(),
         TextColumn(desc),
         transient=True,
     ) as progress:
         task_id = progress.add_task(
```

### Comparing `inferless_cli-1.1.7/inferless_cli/prompts/workspace.py` & `inferless_cli-1.1.8/inferless_cli/prompts/workspace.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/utils/api.py` & `inferless_cli-1.1.8/inferless_cli/utils/api.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/utils/convertors.py` & `inferless_cli-1.1.8/inferless_cli/utils/convertors.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/utils/credentials.py` & `inferless_cli-1.1.8/inferless_cli/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.7/inferless_cli/utils/helpers.py` & `inferless_cli-1.1.8/inferless_cli/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from .constants import (
     DEFAULT_YAML_FILE_NAME,
     DEPLOYMENT_TYPE,
     FRAMEWORKS,
     GLITCHTIP_DSN,
     MACHINE_TYPE_SERVERS,
+    MACHINE_TYPES_REGION_1,
     MACHINE_TYPES_SERVERLESS,
     MODEL_DATA_TYPE_MAPPING,
     MODEL_TRITON_DATA_TYPE_MAPPING,
     REGION_TYPES,
     UPLOAD_METHODS,
     HF_TASK_TYPE,
     HUGGINGFACE_TYPE,
@@ -51,20 +52,22 @@
 import subprocess
 
 yaml = YAML(typ="rt")
 
 key_bindings = KeyBindings()
 
 
-def get_default_machine_values(gpu_type, is_dedicated):
+def get_default_machine_values(gpu_type, is_dedicated, region):
     if is_dedicated not in DEFAULT_MACHINE_VALUES:
         return None
-    if gpu_type not in DEFAULT_MACHINE_VALUES[is_dedicated]:
+    if region not in DEFAULT_MACHINE_VALUES[is_dedicated]:
         return None
-    return DEFAULT_MACHINE_VALUES[is_dedicated][gpu_type]
+    if gpu_type not in DEFAULT_MACHINE_VALUES[is_dedicated][region]:
+        return None
+    return DEFAULT_MACHINE_VALUES[is_dedicated][region][gpu_type]
 
 
 def save_cli_tokens(key, secret):
     if is_keyring_supported():
         try:
             KEYRING.set_password("Inferless", "key", key)
             KEYRING.set_password("Inferless", "secret", secret)
@@ -191,14 +194,21 @@
 def get_machine_types():
     return WordCompleter(
         MACHINE_TYPES,
         ignore_case=True,
     )
 
 
+def get_machine_types_region_1():
+    return WordCompleter(
+        MACHINE_TYPES_REGION_1,
+        ignore_case=True,
+    )
+
+
 def get_machine_types_serverless():
     return WordCompleter(
         MACHINE_TYPES_SERVERLESS,
         ignore_case=True,
     )
```

### Comparing `inferless_cli-1.1.7/inferless_cli/utils/services.py` & `inferless_cli-1.1.8/inferless_cli/utils/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,19 +377,19 @@
 
 def min_version_required():
     try:
         error_statement = "Please update Inferless CLI using [bold][red]`pip install inferless-cli --upgrade`[/red][/bold] \n\n"
         version = get_latest_version()
 
         errmsg, error = compare_versions(__version__, version)
-        if error:
-            rich.print(f"{errmsg} \n\n{error_statement}")
-            raise typer.Exit(1)
     except Exception as e:
         log_exception(e)
+    if error:
+        rich.print(f"{errmsg} \n\n{error_statement}")
+        raise typer.Exit(1)
 
 
 def compare_versions(current_version, latest_version):
     try:
         current_components = list(map(int, current_version.split(".")))
         latest_components = list(map(int, latest_version.split(".")))
```

### Comparing `inferless_cli-1.1.7/inferless_cli/utils/validators.py` & `inferless_cli-1.1.8/inferless_cli/utils/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from prompt_toolkit.validation import ValidationError
 
 from .constants import (
     DEPLOYMENT_TYPE,
     FRAMEWORKS,
     MACHINE_TYPE_SERVERS,
+    MACHINE_TYPES_REGION_1,
     MACHINE_TYPES_SERVERLESS,
     REGION_TYPES,
     UPLOAD_METHODS,
     GITHUB,
     HUGGINGFACE,
     HF_TASK_TYPE,
     HUGGINGFACE_TYPE,
@@ -48,14 +49,23 @@
         raise ValidationError(
             message=f"Invalid choice. Please select from {', '.join(MACHINE_TYPES)}"
         )
     else:
         return choice
 
 
+def validate_machine_types_region_1(choice):
+    if choice not in MACHINE_TYPES_REGION_1:
+        raise ValidationError(
+            message=f"Invalid choice. Please select from {', '.join(MACHINE_TYPES_REGION_1)}"
+        )
+    else:
+        return choice
+
+
 def validate_machine_types_serverless(choice):
     if choice not in MACHINE_TYPES_SERVERLESS:
         raise ValidationError(
             message=f"Invalid choice. Please select from {', '.join(MACHINE_TYPES_SERVERLESS)}"
         )
     else:
         return choice
```

### Comparing `inferless_cli-1.1.7/pyproject.toml` & `inferless_cli-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inferless-cli"
-version = "1.1.7"
+version = "1.1.8"
 description = "Inferless - Deploy Machine Learning Models in Minutes."
 authors = ["Naveen <naveen@inferless.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 inferless = "inferless_cli.main:app"
```

### Comparing `inferless_cli-1.1.7/PKG-INFO` & `inferless_cli-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferless-cli
-Version: 1.1.7
+Version: 1.1.8
 Summary: Inferless - Deploy Machine Learning Models in Minutes.
 Author: Naveen
 Author-email: naveen@inferless.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

