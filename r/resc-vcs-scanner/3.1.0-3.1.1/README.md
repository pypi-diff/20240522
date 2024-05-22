# Comparing `tmp/resc_vcs_scanner-3.1.0.tar.gz` & `tmp/resc_vcs_scanner-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-3.1.0.tar", last modified: Wed May  8 12:38:12 2024, max compression
+gzip compressed data, was "resc_vcs_scanner-3.1.1.tar", last modified: Wed May 22 10:08:21 2024, max compression
```

## Comparing `resc_vcs_scanner-3.1.0.tar` & `resc_vcs_scanner-3.1.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.178023 resc_vcs_scanner-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.182023 resc_vcs_scanner-3.1.0/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/finding_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/ignore_list_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/secret_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.977753 resc_vcs_scanner-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.981753 resc_vcs_scanner-3.1.1/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.981753 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/finding_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/ignore_list_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/secret_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-3.1.0/LICENSE.md` & `resc_vcs_scanner-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.0/PKG-INFO` & `resc_vcs_scanner-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 3.1.0
+Version: 3.1.1
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-3.1.0/README.md` & `resc_vcs_scanner-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.0/setup.cfg` & `resc_vcs_scanner-3.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 3.1.0
+version = 3.1.1
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
```

### Comparing `resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/PKG-INFO` & `resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 3.1.0
+Version: 3.1.1
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/vcs_scanner/__init__.py
 src/vcs_scanner/common.py
 src/vcs_scanner/constants.py
 src/vcs_scanner/input_parser.py
 src/vcs_scanner/model.py
 src/vcs_scanner/resc_worker.py
 src/vcs_scanner/helpers/__init__.py
+src/vcs_scanner/helpers/cli.py
 src/vcs_scanner/helpers/env_default.py
 src/vcs_scanner/helpers/environment_wrapper.py
 src/vcs_scanner/helpers/finding_action.py
 src/vcs_scanner/helpers/finding_filter.py
 src/vcs_scanner/helpers/ignore_list_provider.py
 src/vcs_scanner/secret_scanners/__init__.py
 src/vcs_scanner/secret_scanners/celery_worker.py
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/common.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Standard Library
 import logging.config
 import sys
 import sysconfig
 from os import path
-from typing import Dict, List, Optional
 
 # Third Party
 import tomlkit
 
 # First Party
 from vcs_scanner.input_parser import parse_vcs_instances_file
 from vcs_scanner.model import VCSInstanceRuntime
@@ -82,22 +81,22 @@
     if int(debug) == 1:
         logger_config.setLevel(logging.DEBUG)
     else:
         logger_config.setLevel(logging.INFO)
     return logger_config
 
 
-def load_vcs_instances(file_path: str) -> Dict[str, VCSInstanceRuntime]:
-    vcs_instances_list: List[VCSInstanceRuntime] = parse_vcs_instances_file(file_path)
+def load_vcs_instances(file_path: str) -> dict[str, VCSInstanceRuntime]:
+    vcs_instances_list: list[VCSInstanceRuntime] = parse_vcs_instances_file(file_path)
     if not vcs_instances_list:
         logger.critical(f"Exiting due to issues in VCS Instances definition in file {file_path}")
         sys.exit(-1)
-    vcs_instances_map: Dict[str, VCSInstanceRuntime] = {
+    vcs_instances_map: dict[str, VCSInstanceRuntime] = {
         vcs_instance.name: vcs_instance for vcs_instance in vcs_instances_list
     }
     return vcs_instances_map
 
 
-def get_rule_pack_version_from_file(file_content: str) -> Optional[str]:
+def get_rule_pack_version_from_file(file_content: str) -> str | None:
     toml_rule_dictionary = tomlkit.loads(file_content)
     rule_pack_version = toml_rule_dictionary["version"] if "version" in toml_rule_dictionary else None
     return rule_pack_version
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/env_default.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 class EnvironmentVariable:
     key_name: str
     help_text: str
     default: str = ""
     required: bool = False
 
 
-def validate_environment(env_variables):
+def validate_environment(env_variables: list[EnvironmentVariable]) -> dict[str, EnvironmentVariable]:
     missing = []
     values = {}
     for env_variable in env_variables:
         value = os.environ.get(env_variable.key_name, env_variable.default)
         if not value and env_variable.required:
             missing.append(f"{env_variable.key_name}: {env_variable.help_text}")
         else:
             values[env_variable.key_name] = value
 
     if missing:
-        raise EnvironmentError(f"The following env variables need to be set: {', '.join(missing)}")
+        raise OSError(f"The following env variables need to be set: {', '.join(missing)}")
     return values
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/finding_filter.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/finding_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import tomlkit
 from resc_backend.resc_web_service.schema.finding import FindingCreate
 
 
 def should_process_finding(
     finding: FindingCreate,
     rule_tags: dict = None,
-    include_tags: [str] = None,
-    ignore_tags: [str] = None,
+    include_tags: list[str] = None,
+    ignore_tags: list[str] = None,
 ) -> bool:
     """
         Determine the action to take for the finding, based on the rule tags
     :param finding:
         FindingCreate instance of the finding
     :param rule_tags:
         Dictionary containing all the rules and there respective tags
@@ -29,15 +29,15 @@
     # Rule tag is in the ignore tags list, return false
     if ignore_tags and rule_tags and not set(ignore_tags).isdisjoint(set(rule_tags.get(finding.rule_name, []))):
         return False
 
     return True
 
 
-def get_rule_tags(toml_rule_file_path: str) -> dict:
+def get_rule_tags(toml_rule_file_path: str) -> dict[str, list[str]]:
     """
         Get the tags per rule from the .toml rule file, from self.toml_rule_file_path
     :return: dict.
         The output will contain a dictionary with the rule id as the key and the tags as a list in the value
     """
     rule_tags = {}
     # read toml
@@ -47,19 +47,19 @@
         for toml_rule in toml_rule_dictionary["rules"]:
             rule_id = toml_rule.get("id", None)
             if rule_id:
                 rule_tags[rule_id] = toml_rule.get("tags", [])
     return rule_tags
 
 
-def get_rule_comment(toml_rule_file_path: str) -> dict:
+def get_rule_comment(toml_rule_file_path: str) -> dict[str, str]:
     """
-        Get the tags per rule from the .toml rule file, from self.toml_rule_file_path
+        Get the comment per rule from the .toml rule file, from self.toml_rule_file_path
     :return: dict.
-        The output will contain a dictionary with the rule id as the key and the tags as a list in the value
+        The output will contain a dictionary with the rule id as the key and the comment as a string in the value
     """
     rule_comments = {}
     # read toml
     with open(toml_rule_file_path, encoding="utf-8") as toml_rule_file:
         toml_rule_dictionary = tomlkit.loads(toml_rule_file.read())
         # convert to dict
         for toml_rule in toml_rule_dictionary["rules"]:
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/ignore_list_provider.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/ignore_list_provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,90 @@
 # pylint: disable=E1101
 # Standard Library
 import csv
 import logging
-from datetime import datetime
+from datetime import datetime, UTC
 
 # Third Party
-import dateutil.parser
 
 logger = logging.getLogger(__name__)
 
 
 class IgnoredListProvider:  # pylint: disable=R0902
     def __init__(self, ignore_findings_path: str):
         self.ignore_findings_path: str = ignore_findings_path
-        self.today: datetime = datetime.now()
+        self.today: datetime = datetime.now(UTC)
 
-    def get_ignore_list(self) -> dict:
+    def get_ignore_list(self) -> dict[str, True]:
         """
         Get the dictionary of ignored findings according to the file
-        The output will contain a dictionary with the findings id as the key and the tags as a list in the value
+        The output will contain a dictionary with the path|rule|line as key and True as value.
+        We use a dictionary for random access instead of list.
         """
-        ignored = {}
-
         if self.ignore_findings_path is None:
-            return ignored
+            return {}
+
+        ignored = {}
 
         try:
             # read dsv: `path|rule_name|line_number|expiry_date`
             with open(self.ignore_findings_path, encoding="utf-8") as ignore_findings_file:
                 csv_ignore_list = csv.reader(ignore_findings_file, delimiter="|")
                 for row in csv_ignore_list:
-                    expire: datetime = datetime.now()
+                    if self._is_row_comment(row):
+                        continue
 
-                    # rows starting with # are comments
-                    if row[0][:1] == "#":
+                    if not self._is_row_valid(row):
                         continue
 
-                    if len(row) < 3:
-                        string_row: str = "".join(row)
-                        logger.warning(f"Skipping: incomplete entry for {string_row}")
+                    if not self._is_row_active(row):
                         continue
 
+                    # we use the path, rule_name, line_number as a dictionary key
                     path = row[0]
                     rule = row[1]
                     line = row[2]
-                    if len(row) > 3:
-                        date = row[3]
-                        try:
-                            expire: datetime = dateutil.parser.isoparse(date)
-                        except ValueError:
-                            logger.warning(f"Skipping: invalid date entry for {path}: {date}")
-                            continue
-
-                    if expire < self.today:
-                        logger.warning(f"Info: expired date entry for {date}")
-                        continue
-
-                    # we use the path, rule_name, line_number as a dictionary key
                     ignored[f"{path}|{rule}|{line}"] = True
         except FileNotFoundError:  # <- File does not exists: we just fail silently
             logger.warning(f"could not find {self.ignore_findings_path}")
             return {}
 
         return ignored
+
+    def _is_row_comment(self, row: list[str]) -> bool:
+        """
+        Line starting with # are comments
+        """
+        return row[0][:1] == "#"
+
+    def _is_row_valid(self, row: list[str]) -> bool:
+        """
+        If a line is strictly shorter than 3, it is not a valid entry
+        """
+        if len(row) >= 3:
+            return True
+
+        string_row: str = "".join(row)
+        logger.warning(f"Skipping: incomplete entry for {string_row}")
+        return False
+
+    def _is_row_active(self, row: list[str]) -> bool:
+        """
+        A row is active if it is of length 3 or if the date of the row is not in the past.
+        """
+        if len(row) == 3:
+            return True
+
+        path = row[0]
+        date = row[3]
+        try:
+            expire: datetime = datetime.fromisoformat(date).replace(tzinfo=UTC)
+
+        except ValueError:
+            logger.warning(f"Skipping: invalid date entry for {path}: {date}")
+            return False
+
+        if expire < self.today:
+            logger.warning(f"Info: expired date entry for {date}")
+            return False
+
+        return True
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/input_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Standard Library
 import json
 import logging
 from json import JSONDecodeError
-from typing import List
 
 # Third Party
 from pydantic import ValidationError
 
 # First Party
 from vcs_scanner.model import VCSInstanceRuntime
 
 logger = logging.getLogger(__name__)
 
 
-def parse_vcs_instances_file(filepath: str) -> List[VCSInstanceRuntime]:
-    vcs_instances: List[VCSInstanceRuntime] = []
+def parse_vcs_instances_file(filepath: str) -> list[VCSInstanceRuntime]:
+    vcs_instances: list[VCSInstanceRuntime] = []
     errors_found = False
     logging.info(f"Reading VCS instances from file {filepath}")
     try:
         with open(filepath, encoding="utf-8") as vcs_instances_file:
             parsed_vcs_instances = json.loads(vcs_instances_file.read())
             logging.info(f"Parsing VCS instance definitions from file {filepath}")
             for vcs_instance in parsed_vcs_instances:
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/model.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 # pylint: disable=no-name-in-module
 # Standard Library
 import os
-from typing import List, Optional
 
 # Third Party
 from pydantic import BaseModel, conint, constr, validator
 from resc_backend.resc_web_service.schema.repository import Repository
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 
 class RepositoryRuntime(BaseModel):
     repository_name: str
     repository_id: str
     repository_url: str
     project_key: str
     vcs_instance_name: str
-    latest_commit: Optional[str] = None
+    latest_commit: str | None = None
 
     def convert_to_repository(self, vcs_instance_id: int) -> Repository:
         return Repository(
             project_key=self.project_key,
             repository_id=self.repository_id,
             repository_name=self.repository_name,
             repository_url=self.repository_url,
             vcs_instance=vcs_instance_id,
             latest_commit=self.latest_commit,
         )
 
 
 class VCSInstanceRuntime(BaseModel):
-    id_: Optional[int]
+    id_: int | None
     name: constr(max_length=200)
     provider_type: VCSProviders
     hostname: constr(max_length=200)
     port: conint(gt=-0, lt=65536)
     scheme: str
     username: constr(max_length=200)
     token: constr(max_length=200)
-    exceptions: Optional[List[str]] = []
-    scope: Optional[List[str]] = []
-    organization: Optional[str]
+    exceptions: list[str] | None = []
+    scope: list[str] | None = []
+    organization: str | None
 
     @validator("scheme", pre=True)
     @classmethod
     def check_scheme(cls, value):
         allowed_schemes = ["http", "https"]
         if value not in allowed_schemes:
             raise ValueError(f"The scheme '{value}' must be one of the following {', '.join(allowed_schemes)}")
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/git_operation.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/git_operation.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Standard Library
-import datetime
+from datetime import datetime, UTC
 import json
 import logging
 import subprocess
-from typing import List, Optional
 
 # Third Party
 from resc_backend.resc_web_service.schema.finding import FindingBase
 
 # First Party
 from vcs_scanner.constants import LEAKS_FOUND_EXIT_CODE, NO_LEAKS_FOUND_EXIT_CODE
 
@@ -48,26 +47,25 @@
             command.append("--no-git")
 
         # Incremental scan command
         if self.scan_from:
             command.append(f"--log-opts={self.scan_from}..")
         return command
 
-    def start_scan(self) -> Optional[List[FindingBase]]:
+    def start_scan(self) -> list[FindingBase] | None:
         """
         :return: Output.
             If Successful, a list of FindingCreate objects is returned.
             Otherwise, a None object is returned
         """
         try:
             result = subprocess.run(
                 self._build_gitleaks_command(),
                 check=False,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
+                capture_output=True,
             )
 
             exitcode = result.returncode
             if exitcode == NO_LEAKS_FOUND_EXIT_CODE:
                 return []
             if exitcode == LEAKS_FOUND_EXIT_CODE:
                 return self._parse_output(self.report_filepath)
@@ -106,39 +104,37 @@
         new_url = new_url.replace("/blob/", "/commits/")
         new_url = new_url.replace(f"/{repository}/", f"/repos/{repository[:-4]}/")  # remove .git at the end
         new_url = new_url.replace(f"/{commit_id}/", f"/{commit_id}#")
 
         return new_url
 
     @staticmethod
-    def _is_valid_timestamp(timestamp: str) -> Optional[datetime.datetime]:
+    def _is_valid_timestamp(timestamp: str) -> datetime | None:
         try:
-            converted_timestamp: Optional[datetime.datetime] = datetime.datetime.strptime(
-                timestamp, "%Y-%m-%dT%H:%M:%S%z"
-            )
+            converted_timestamp: datetime | None = datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%S%z")
         except ValueError:
             converted_timestamp = None
         return converted_timestamp
 
     @classmethod
-    def _parse_output(cls, file_path: str) -> List[FindingBase]:
+    def _parse_output(cls, file_path: str) -> list[FindingBase]:
         """
         Parse the gitleaks findings from the temp file and return a list of Finding objects
         :param file_path: the tempfile containing the gitleaks findings
         :return: list of Finding objects
         """
         findings = []
         with open(file_path, encoding="utf-8") as report_file:
             results = json.load(report_file)
 
         for result in results:
             commit_timestamp = cls._is_valid_timestamp(result["Date"])
             if not commit_timestamp:
                 logger.debug(f"{result['Date']} has an unexpected date format. Expected ISO 8601")
-                commit_timestamp = datetime.datetime.now()
+                commit_timestamp = datetime.now(UTC)
             finding = FindingBase(
                 file_path=result["File"],
                 line_number=result["StartLine"],
                 column_start=result["StartColumn"],
                 column_end=result["EndColumn"],
                 email=result["Email"],
                 author=result["Author"],
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # pylint: disable=E1101
 # Standard Library
 import logging
 import os
 import shutil
 import time
 import uuid
-from datetime import datetime
-from typing import List, Optional
+from datetime import datetime, UTC
 
 # Third Party
 from resc_backend.resc_web_service.schema.finding import FindingBase
 from resc_backend.resc_web_service.schema.repository import Repository
 from resc_backend.resc_web_service.schema.scan import Scan
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
@@ -100,15 +99,15 @@
         scan_type_to_run = self.determine_scan_type(
             latest_commit=self.latest_commit,
             last_scan_for_repository=last_scan_for_repository,
         )
 
         if scan_type_to_run:
             # Insert in to scan table
-            scan_timestamp_start = datetime.utcnow()
+            scan_timestamp_start = datetime.now(UTC)
             created_scan = self._output_module.write_scan(
                 scan_type_to_run,
                 self.latest_commit,
                 scan_timestamp_start.isoformat(),
                 created_repository,
                 rule_pack=self.rule_pack_version,
             )
@@ -122,15 +121,15 @@
             # Clone and run scan upon the repository
             if not self.local_path:
                 repo_clone_path: str = self.clone_repo()
             else:
                 repo_clone_path = self.local_path
 
             findings = self.scan_repo(scan_type_to_run, last_scanned_commit, repo_clone_path)
-            scan_timestamp_end = datetime.utcnow()
+            scan_timestamp_end = datetime.now(UTC)
             logger.info(
                 f"Running {scan_type_to_run} scan on repository "
                 f"{self.repository.project_key}/{self.repository.repository_name}"
                 f" took {scan_timestamp_end - scan_timestamp_start} ms."
             )
 
             if findings:
@@ -152,28 +151,28 @@
 
     def run_directory_scan(self) -> None:
         """
         Scan the given non-git directory, set in the self.local_path variable
         """
         logger.info(f"Started task for scanning {self.local_path} using rule pack version: {self.rule_pack_version}")
 
-        scan_timestamp_start = datetime.utcnow()
+        scan_timestamp_start = datetime.now(UTC)
         findings = self.scan_directory(self.local_path)
-        scan_timestamp_end = datetime.utcnow()
+        scan_timestamp_end = datetime.now(UTC)
         logger.info(f"Running local scan on {self.local_path} took {scan_timestamp_end - scan_timestamp_start} ms.")
 
         if findings:
             logger.info(f"Scan completed: {len(findings)} findings were found.")
             self._output_module.write_findings(repository_id=0, scan_id=0, scan_findings=findings)
         else:
             logger.info(f"No findings registered in {self.local_path}.")
 
     def scan_repo(
         self, scan_type_to_run: str, last_scanned_commit: str, repo_clone_path: str
-    ) -> Optional[List[FindingBase]]:
+    ) -> list[FindingBase] | None:
         """
             Clone and scan the given repository
         :param repo_clone_path:
             Directory path where the repository has already been cloned
         :param scan_type_to_run:
             Type of scan to run (Base or Incremental)
         :param last_scanned_commit:
@@ -201,15 +200,15 @@
                 gitleaks_path=self.gitleaks_binary_path,
                 repository_path=repo_clone_path,
                 rules_filepath=self.gitleaks_rules_path,
                 report_filepath=report_filepath,
             )
 
             before_scan = time.time()
-            findings: Optional[List[FindingBase]] = gitleaks_command.start_scan()
+            findings: list[FindingBase] | None = gitleaks_command.start_scan()
             after_scan = time.time()
             scan_duration = int(after_scan - before_scan)
             logger.info(f"scan of repository {repo_clone_path} took {scan_duration} seconds")
             return findings
         except BaseException as error:
             logger.error(
                 f"An exception occurred while scanning repository {self.repository.repository_url} " f"error: {error}"
@@ -220,15 +219,15 @@
             if os.path.exists(report_filepath):
                 os.remove(report_filepath)
             if repo_clone_path and not self.local_path and os.path.exists(repo_clone_path):
                 logger.debug(f"Cleaning up the repository cloned directory: {repo_clone_path}")
                 shutil.rmtree(repo_clone_path)
         return None
 
-    def scan_directory(self, directory_path: str) -> Optional[List[FindingBase]]:
+    def scan_directory(self, directory_path: str) -> list[FindingBase] | None:
         """
             Scan the given directory
         :param directory_path:
             Directory path to be scanned
         :return: Optional[List[FindingBase]].
             The output will contain a list of findings or an empty list if no finding was found
         """
@@ -244,15 +243,15 @@
                 repository_path=directory_path,
                 rules_filepath=self.gitleaks_rules_path,
                 report_filepath=report_filepath,
                 git_scan=False,
             )
 
             before_scan = time.time()
-            findings: Optional[List[FindingBase]] = gitleaks_command.start_scan()
+            findings: list[FindingBase] | None = gitleaks_command.start_scan()
             after_scan = time.time()
             scan_duration = int(after_scan - before_scan)
             logger.info(f"scan of repository {directory_path} took {scan_duration} seconds")
             return findings
         except BaseException as error:
             logger.error(f"An exception occurred while scanning directory {directory_path} error: {error}")
         finally:
```

### Comparing `resc_vcs_scanner-3.1.0/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-3.1.1/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*

