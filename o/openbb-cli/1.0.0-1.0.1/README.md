# Comparing `tmp/openbb_cli-1.0.0.tar.gz` & `tmp/openbb_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_cli-1.0.0.tar", max compression
+gzip compressed data, was "openbb_cli-1.0.1.tar", max compression
```

## Comparing `openbb_cli-1.0.0.tar` & `openbb_cli-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     2737 2024-05-14 15:30:05.601425 openbb_cli-1.0.0/README.md
--rw-r--r--   0        0        0       19 2024-05-09 13:34:29.156403 openbb_cli-1.0.0/openbb_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 13:34:29.156460 openbb_cli-1.0.0/openbb_cli/argparse_translator/__init__.py
--rw-r--r--   0        0        0     4766 2024-05-15 17:16:12.291662 openbb_cli-1.0.0/openbb_cli/argparse_translator/argparse_class_processor.py
--rw-r--r--   0        0        0    23229 2024-05-15 17:16:12.291996 openbb_cli-1.0.0/openbb_cli/argparse_translator/argparse_translator.py
--rw-r--r--   0        0        0     3479 2024-05-14 15:30:05.601842 openbb_cli-1.0.0/openbb_cli/argparse_translator/obbject_registry.py
--rw-r--r--   0        0        0      439 2024-05-09 13:34:29.158084 openbb_cli-1.0.0/openbb_cli/assets/routines/routine_example.openbb
--rw-r--r--   0        0        0   358460 2024-05-09 13:34:29.160915 openbb_cli-1.0.0/openbb_cli/assets/styles/default/Consolas.ttf
--rw-r--r--   0        0        0      972 2024-05-09 13:34:29.161055 openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.mpfstyle.json
--rw-r--r--   0        0        0      182 2024-05-09 13:34:29.161131 openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.mplrc.json
--rw-r--r--   0        0        0     2086 2024-05-09 13:34:29.161224 openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.mplstyle
--rw-r--r--   0        0        0     3204 2024-05-09 13:34:29.161910 openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0      203 2024-05-09 13:34:29.161999 openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.richstyle.json
--rw-r--r--   0        0        0      970 2024-05-09 13:34:29.162072 openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.mpfstyle.json
--rw-r--r--   0        0        0      182 2024-05-09 13:34:29.162136 openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.mplrc.json
--rw-r--r--   0        0        0     2035 2024-05-09 13:34:29.162207 openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.mplstyle
--rw-r--r--   0        0        0    23603 2024-05-09 13:34:29.162291 openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0      202 2024-05-09 13:34:29.162368 openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.richstyle.json
--rw-r--r--   0        0        0     2505 2024-05-09 13:34:29.162649 openbb_cli-1.0.0/openbb_cli/assets/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0      186 2024-05-09 13:34:29.162734 openbb_cli-1.0.0/openbb_cli/assets/styles/user/openbb.richstyle.json
--rw-r--r--   0        0        0      377 2024-05-09 13:34:29.163206 openbb_cli-1.0.0/openbb_cli/cli.py
--rw-r--r--   0        0        0       24 2024-05-09 13:34:29.163289 openbb_cli-1.0.0/openbb_cli/config/__init__.py
--rw-r--r--   0        0        0    17847 2024-05-15 17:16:12.293241 openbb_cli-1.0.0/openbb_cli/config/completer.py
--rw-r--r--   0        0        0     3020 2024-05-15 17:16:12.293460 openbb_cli-1.0.0/openbb_cli/config/console.py
--rw-r--r--   0        0        0     1811 2024-05-13 09:44:02.287284 openbb_cli-1.0.0/openbb_cli/config/constants.py
--rw-r--r--   0        0        0     5434 2024-05-15 17:16:12.293676 openbb_cli-1.0.0/openbb_cli/config/menu_text.py
--rw-r--r--   0        0        0      319 2024-05-13 11:24:09.208924 openbb_cli-1.0.0/openbb_cli/config/setup.py
--rw-r--r--   0        0        0     3537 2024-05-15 17:16:12.293811 openbb_cli-1.0.0/openbb_cli/config/style.py
--rw-r--r--   0        0        0    35379 2024-05-15 17:16:12.294395 openbb_cli-1.0.0/openbb_cli/controllers/base_controller.py
--rw-r--r--   0        0        0    13687 2024-05-15 17:16:12.294762 openbb_cli-1.0.0/openbb_cli/controllers/base_platform_controller.py
--rw-r--r--   0        0        0     9697 2024-05-15 17:16:12.295014 openbb_cli-1.0.0/openbb_cli/controllers/choices.py
--rw-r--r--   0        0        0    34231 2024-05-15 17:16:12.295370 openbb_cli-1.0.0/openbb_cli/controllers/cli_controller.py
--rw-r--r--   0        0        0     3364 2024-05-09 13:34:29.166860 openbb_cli-1.0.0/openbb_cli/controllers/hub_service.py
--rw-r--r--   0        0        0     2098 2024-05-09 13:34:29.167341 openbb_cli-1.0.0/openbb_cli/controllers/platform_controller_factory.py
--rw-r--r--   0        0        0    20452 2024-05-15 17:16:12.295611 openbb_cli-1.0.0/openbb_cli/controllers/script_parser.py
--rw-r--r--   0        0        0    12776 2024-05-15 17:16:12.296213 openbb_cli-1.0.0/openbb_cli/controllers/settings_controller.py
--rw-r--r--   0        0        0    31575 2024-05-15 17:16:12.296928 openbb_cli-1.0.0/openbb_cli/controllers/utils.py
--rw-r--r--   0        0        0     2116 2024-05-10 19:27:56.003307 openbb_cli-1.0.0/openbb_cli/models/settings.py
--rw-r--r--   0        0        0     2762 2024-05-10 19:27:56.003476 openbb_cli-1.0.0/openbb_cli/session.py
--rw-r--r--   0        0        0      850 2024-05-15 17:50:34.248749 openbb_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 openbb_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2751 2024-05-22 11:48:40.387330 openbb_cli-1.0.1/README.md
+-rw-r--r--   0        0        0       19 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/argparse_translator/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-22 13:43:16.380975 openbb_cli-1.0.1/openbb_cli/argparse_translator/argparse_class_processor.py
+-rw-r--r--   0        0        0    23226 2024-05-22 13:43:16.380975 openbb_cli-1.0.1/openbb_cli/argparse_translator/argparse_translator.py
+-rw-r--r--   0        0        0     3479 2024-05-15 09:21:56.009885 openbb_cli-1.0.1/openbb_cli/argparse_translator/obbject_registry.py
+-rw-r--r--   0        0        0      439 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/routines/routine_example.openbb
+-rw-r--r--   0        0        0   358460 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/Consolas.ttf
+-rw-r--r--   0        0        0      972 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.mpfstyle.json
+-rw-r--r--   0        0        0      182 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.mplrc.json
+-rw-r--r--   0        0        0     2086 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.mplstyle
+-rw-r--r--   0        0        0     3204 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0      203 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.richstyle.json
+-rw-r--r--   0        0        0      970 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.mpfstyle.json
+-rw-r--r--   0        0        0      182 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.mplrc.json
+-rw-r--r--   0        0        0     2035 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.mplstyle
+-rw-r--r--   0        0        0    23603 2024-05-14 16:57:23.522032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0      202 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.richstyle.json
+-rw-r--r--   0        0        0     2505 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/assets/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0      186 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/assets/styles/user/openbb.richstyle.json
+-rw-r--r--   0        0        0      481 2024-05-22 11:48:40.387330 openbb_cli-1.0.1/openbb_cli/cli.py
+-rw-r--r--   0        0        0       24 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/config/__init__.py
+-rw-r--r--   0        0        0    17847 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/config/completer.py
+-rw-r--r--   0        0        0     3020 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/config/console.py
+-rw-r--r--   0        0        0     1811 2024-05-15 09:21:56.009885 openbb_cli-1.0.1/openbb_cli/config/constants.py
+-rw-r--r--   0        0        0     5434 2024-05-15 11:30:49.635743 openbb_cli-1.0.1/openbb_cli/config/menu_text.py
+-rw-r--r--   0        0        0      319 2024-05-15 09:21:56.009885 openbb_cli-1.0.1/openbb_cli/config/setup.py
+-rw-r--r--   0        0        0     3537 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/config/style.py
+-rw-r--r--   0        0        0    35785 2024-05-22 13:43:16.380975 openbb_cli-1.0.1/openbb_cli/controllers/base_controller.py
+-rw-r--r--   0        0        0    13686 2024-05-22 13:43:16.380975 openbb_cli-1.0.1/openbb_cli/controllers/base_platform_controller.py
+-rw-r--r--   0        0        0     9705 2024-05-22 11:48:40.387330 openbb_cli-1.0.1/openbb_cli/controllers/choices.py
+-rw-r--r--   0        0        0    34367 2024-05-22 13:43:16.380975 openbb_cli-1.0.1/openbb_cli/controllers/cli_controller.py
+-rw-r--r--   0        0        0     3364 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/controllers/hub_service.py
+-rw-r--r--   0        0        0     2098 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/controllers/platform_controller_factory.py
+-rw-r--r--   0        0        0    20452 2024-05-14 16:57:23.526032 openbb_cli-1.0.1/openbb_cli/controllers/script_parser.py
+-rw-r--r--   0        0        0    12776 2024-05-15 11:30:49.635743 openbb_cli-1.0.1/openbb_cli/controllers/settings_controller.py
+-rw-r--r--   0        0        0    31703 2024-05-22 11:48:40.387330 openbb_cli-1.0.1/openbb_cli/controllers/utils.py
+-rw-r--r--   0        0        0     2116 2024-05-15 09:21:56.009885 openbb_cli-1.0.1/openbb_cli/models/settings.py
+-rw-r--r--   0        0        0     2762 2024-05-15 09:21:56.009885 openbb_cli-1.0.1/openbb_cli/session.py
+-rw-r--r--   0        0        0      780 2024-05-22 14:04:53.097329 openbb_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 openbb_cli-1.0.1/PKG-INFO
```

### Comparing `openbb_cli-1.0.0/README.md` & `openbb_cli-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 | OpenBB is committed to build the future of investment research by focusing on an open source infrastructure accessible to everyone, everywhere. |
 | :---------------------------------------------------------------------------------------------------------------------------------------------: |
 |              ![OpenBBLogo](https://user-images.githubusercontent.com/25267873/218899768-1f0964b8-326c-4f35-af6f-ea0946ac970b.png)               |
 |                                                 Check our website at [openbb.co](www.openbb.co)                                                 |
 
 ## Overview
 
-The OpenBB CLI is a command line interface that wraps [OpenBB Platform](https://docs.openbb.co/platform).
+The OpenBB Platform CLI is a command line interface that wraps [OpenBB Platform](https://docs.openbb.co/platform).
 
 It offers a convenient way to interact with the OpenBB Platform and its extensions, as well as automate data collection via OpenBB Routine Scripts.
 
-Find the most complete documentation, examples, and usage guides for the OpenBB Platform CLI [here](https://my.openbb.co/app/cli).
+Find the most complete documentation, examples, and usage guides for the OpenBB Platform CLI [here](https://docs.openbb.co/cli).
 
 ## Installation
 
 The command below provides access to the all the available OpenBB extensions behind the OpenBB Platform, find the complete list [here](https://my.openbb.co/app/platform/extensions).
 
 ```bash
 pip install openbb-cli
 ```
 
-> Note: Find the most complete installation hints and tips [here](https://my.openbb.co/app/cli/installation).
+> Note: Find the most complete installation hints and tips [here](https://docs.openbb.co/cli/installation).
 
-After the installation is complete, you can deploy the OpenBB CLI by running the following command:
+After the installation is complete, you can deploy the OpenBB Platform CLI by running the following command:
 
 ```bash
 openbb
 ```
 
 Which should result in the following output:
```

### Comparing `openbb_cli-1.0.0/openbb_cli/argparse_translator/argparse_class_processor.py` & `openbb_cli-1.0.1/openbb_cli/argparse_translator/argparse_class_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     ) -> Dict[str, ArgparseTranslator]:
         methods = {}
 
         for name, member in inspect.getmembers(target):
             if name.startswith("__") or name.startswith("_"):
                 continue
             if inspect.ismethod(member):
-
                 class_name = cls._get_class_name(target)
                 methods[f"{class_name}_{name}"] = ArgparseTranslator(
                     func=member,
                     add_help=add_help,
                     custom_argument_groups=cls._custom_groups_from_reference(  # type: ignore
                         class_name=class_name, function_name=name
                     ),
```

### Comparing `openbb_cli-1.0.0/openbb_cli/argparse_translator/argparse_translator.py` & `openbb_cli-1.0.1/openbb_cli/argparse_translator/argparse_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 class ArgparseActionType(Enum):
     store = "store"
     store_true = "store_true"
 
 
 class CustomArgument(BaseModel):
-
     name: str
     type: Optional[Any]
     dest: str
     default: Any
     required: bool
     action: Literal["store_true", "store"]
     help: str
@@ -58,15 +57,14 @@
             values.type = None
             values.nargs = None
             values.choices = None
         return values
 
     # override
     def model_dump(self, **kwargs):
-
         res = super().model_dump(**kwargs)
 
         # Check if choices is present and if it's an empty tuple remove it
         if "choices" in res and not res["choices"]:
             del res["choices"]
 
         return res
@@ -148,15 +146,14 @@
             return tuple(custom_choices)
 
         return choices
 
     def build_custom_groups(self):
         """Build the custom groups from the reference."""
         for route, v in self.reference.items():
-
             for provider, args in v["parameters"].items():
                 if provider == "standard":
                     continue
 
                 custom_arguments = []
                 for arg in args:
                     if arg.get("standard"):
```

### Comparing `openbb_cli-1.0.0/openbb_cli/argparse_translator/obbject_registry.py` & `openbb_cli-1.0.1/openbb_cli/argparse_translator/obbject_registry.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/Consolas.ttf` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/Consolas.ttf`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.mpfstyle.json` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.mplstyle` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/dark.pltstyle.json` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.mpfstyle.json` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.mplstyle` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/light.pltstyle.json` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/assets/styles/default/tables.pltstyle.json` & `openbb_cli-1.0.1/openbb_cli/assets/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/config/completer.py` & `openbb_cli-1.0.1/openbb_cli/config/completer.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/config/console.py` & `openbb_cli-1.0.1/openbb_cli/config/console.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/config/constants.py` & `openbb_cli-1.0.1/openbb_cli/config/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/config/menu_text.py` & `openbb_cli-1.0.1/openbb_cli/config/menu_text.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/config/style.py` & `openbb_cli-1.0.1/openbb_cli/config/style.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/base_controller.py` & `openbb_cli-1.0.1/openbb_cli/controllers/base_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Base controller for the CLI."""
 
 import argparse
 import difflib
 import os
 import re
+import shlex
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Union
 
 import pandas as pd
 from openbb_cli.config.completer import NestedCompleter
@@ -236,15 +237,15 @@
                 if cmd:
                     self.queue.insert(0, cmd)
 
         # Single command fed, process
         else:
             try:
                 (known_args, other_args) = self.parser.parse_known_args(
-                    an_input.split()
+                    shlex.split(an_input)
                 )
             except Exception as exc:
                 raise SystemExit from exc
 
             if RECORD_SESSION:
                 SESSION_RECORDED.append(an_input)
 
@@ -740,19 +741,19 @@
             choices_export = []
             help_export = "Does not export!"
 
             if export_allowed == "raw_data_only":
                 choices_export = ["csv", "json", "xlsx"]
                 help_export = "Export raw data into csv, json, xlsx"
             elif export_allowed == "figures_only":
-                choices_export = ["png", "jpg", "pdf", "svg"]
-                help_export = "Export figure into png, jpg, pdf, svg "
+                choices_export = ["png", "jpg", "svg"]
+                help_export = "Export figure into png, jpg, svg "
             else:
-                choices_export = ["csv", "json", "xlsx", "png", "jpg", "pdf", "svg"]
-                help_export = "Export raw data into csv, json, xlsx and figure into png, jpg, pdf, svg "
+                choices_export = ["csv", "json", "xlsx", "png", "jpg", "svg"]
+                help_export = "Export raw data into csv, json, xlsx and figure into png, jpg, svg "
 
             parser.add_argument(
                 "--export",
                 default="",
                 type=check_file_type_saved(choices_export),
                 dest="export",
                 help=help_export,
@@ -794,28 +795,39 @@
 
         if "--help" in other_args or "-h" in other_args:
             txt_help = parser.format_help() + "\n"
             session.console.print(f"[help]{txt_help}[/help]")
             return None
 
         try:
-            # If the user uses a comma separated list of arguments, split them
-            for index, arg in enumerate(other_args):
-                if "," in arg:
-                    parts = arg.split(",")
-                    other_args[index : index + 1] = parts
+            # Determine the index of the routine arguments
+            routine_args_index = next(
+                (
+                    i + 1
+                    for i, arg in enumerate(other_args)
+                    if arg in ("-i", "--input")
+                    and "routine_args" in [action.dest for action in parser._actions]
+                ),
+                -1,
+            )
+            # Split comma-separated arguments, except for the argument at routine_args_index
+            other_args = [
+                part
+                for index, arg in enumerate(other_args)
+                for part in (arg.split(",") if index != routine_args_index else [arg])
+            ]
 
             (ns_parser, l_unknown_args) = parser.parse_known_args(other_args)
 
             if export_allowed in [
                 "raw_data_only",
                 "raw_data_and_figures",
             ]:
                 ns_parser.is_image = any(
-                    ext in ns_parser.export for ext in ["png", "svg", "jpg", "pdf"]
+                    ext in ns_parser.export for ext in ["png", "svg", "jpg"]
                 )
 
         except SystemExit:
             # In case the command has required argument that isn't specified
 
             return None
```

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/base_platform_controller.py` & `openbb_cli-1.0.1/openbb_cli/controllers/base_platform_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,14 @@
 
                     obbject = translator.execute_func(parsed_args=ns_parser)
                     df: pd.DataFrame = pd.DataFrame()
                     fig: OpenBBFigure = None
                     title = f"{self.PATH}{translator.func.__name__}"
 
                     if obbject:
-
                         if isinstance(obbject, OBBject):
                             if session.max_obbjects_exceeded() and obbject.results:
                                 session.obbject_registry.remove()
                                 session.console.print(
                                     "[yellow]Maximum number of OBBjects reached. The oldest entry was removed.[yellow]"
                                 )
```

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/choices.py` & `openbb_cli-1.0.1/openbb_cli/controllers/choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,19 +54,21 @@
         choices_export = []
         help_export = "Does not export!"
 
         if export_allowed == "raw_data_only":
             choices_export = ["csv", "json", "xlsx"]
             help_export = "Export raw data into csv, json, xlsx"
         elif export_allowed == "figures_only":
-            choices_export = ["png", "jpg", "pdf", "svg"]
-            help_export = "Export figure into png, jpg, pdf, svg "
+            choices_export = ["png", "jpg", "svg"]
+            help_export = "Export figure into png, jpg, svg "
         else:
-            choices_export = ["csv", "json", "xlsx", "png", "jpg", "pdf", "svg"]
-            help_export = "Export raw data into csv, json, xlsx and figure into png, jpg, pdf, svg "
+            choices_export = ["csv", "json", "xlsx", "png", "jpg", "svg"]
+            help_export = (
+                "Export raw data into csv, json, xlsx and figure into png, jpg, svg "
+            )
 
         parser.add_argument(
             "--export",
             default="",
             type=check_file_type_saved(choices_export),
             dest="export",
             help=help_export,
```

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/cli_controller.py` & `openbb_cli-1.0.1/openbb_cli/controllers/cli_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
             nargs="+",
         )
         parser.add_argument(
             "-i",
             "--input",
             help="Select multiple inputs to be replaced in the routine and separated by commas. E.g. GME,AMC,BTC-USD",
             dest="routine_args",
-            type=lambda s: [str(item) for item in s.split(",")],
+            type=str,
         )
         parser.add_argument(
             "-e",
             "--example",
             help="Run an example script to understand how routines can be used.",
             dest="example",
             action="store_true",
@@ -427,25 +427,30 @@
             else:
                 return
 
             try:
                 with open(routine_path) as fp:
                     raw_lines = list(fp)
 
+                script_inputs = []
                 # Capture ARGV either as list if args separated by commas or as single value
-                if ns_parser.routine_args:
-                    script_inputs = (
-                        ns_parser.routine_args
-                        if "," not in ns_parser.routine_args
-                        else ns_parser.routine_args.split(",")
+                if routine_args := ns_parser.routine_args:
+                    pattern = r"\[(.*?)\]"
+                    matches = re.findall(pattern, routine_args)
+
+                    for match in matches:
+                        routine_args = routine_args.replace(f"[{match}]", "")
+                        script_inputs.append(match)
+
+                    script_inputs.extend(
+                        [val for val in routine_args.split(",") if val]
                     )
 
                 err, parsed_script = parse_openbb_script(
-                    raw_lines=raw_lines,
-                    script_inputs=script_inputs if ns_parser.routine_args else None,
+                    raw_lines=raw_lines, script_inputs=script_inputs
                 )
 
                 # If there err output is not an empty string then it means there was an
                 # issue in parsing the routine and therefore we don't want to feed it
                 # to the terminal
                 if err:
                     session.console.print(err)
@@ -542,15 +547,14 @@
         if first_time_user():
             with contextlib.suppress(EOFError):
                 webbrowser.open("https://docs.openbb.co/cli")
 
         t_controller.print_help()
 
     while ret_code:
-
         # There is a command in the queue
         if t_controller.queue and len(t_controller.queue) > 0:
             # If the command is quitting the menu we want to return in here
             if t_controller.queue[0] in ("q", "..", "quit"):
                 print_goodbye()
                 break
```

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/hub_service.py` & `openbb_cli-1.0.1/openbb_cli/controllers/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/platform_controller_factory.py` & `openbb_cli-1.0.1/openbb_cli/controllers/platform_controller_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/script_parser.py` & `openbb_cli-1.0.1/openbb_cli/controllers/script_parser.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/settings_controller.py` & `openbb_cli-1.0.1/openbb_cli/controllers/settings_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/controllers/utils.py` & `openbb_cli-1.0.1/openbb_cli/controllers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -897,24 +897,27 @@
                         saved_path,
                         index=True,
                         header=True,
                     )
                 else:
                     save_to_excel(df, saved_path, sheet_name)
 
-            elif saved_path.suffix in [".jpg", ".pdf", ".png", ".svg"]:
+            elif saved_path.suffix in [".jpg", ".png", ".svg"]:
                 if figure is None:
                     Session().console.print("No plot to export.")
                     continue
                 figure.show(export_image=saved_path, margin=margin)
             else:
                 Session().console.print("Wrong export file specified.")
                 continue
 
-            Session().console.print(f"Saved file: {saved_path}")
+            if saved_path.exists():
+                Session().console.print(f"Saved file: {saved_path}")
+            else:
+                Session().console.print(f"Failed to save file: {saved_path}")
 
         if figure is not None:
             figure._exported = True  # pylint: disable=protected-access
 
 
 def system_clear():
     """Clear screen."""
```

### Comparing `openbb_cli-1.0.0/openbb_cli/models/settings.py` & `openbb_cli-1.0.1/openbb_cli/models/settings.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/openbb_cli/session.py` & `openbb_cli-1.0.1/openbb_cli/session.py`

 * *Files identical despite different names*

### Comparing `openbb_cli-1.0.0/pyproject.toml` & `openbb_cli-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "Investment Research for Everyone, Anywhere."
 authors = ["OpenBB <hello@openbb.co>"]
 packages = [{ include = "openbb_cli" }]
 license = "AGPL-3.0-only"
 readme = "README.md"
 homepage = "https://openbb.co"
 repository = "https://github.com/OpenBB-finance/OpenBBTerminal"
@@ -13,21 +13,18 @@
 [tool.poetry.scripts]
 openbb = 'openbb_cli.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.12"
 
 # OpenBB dependencies
-openbb = { version = "^4.2.0", extras = ["all"] }
+openbb = { version = "^4.2.1", extras = ["all"] }
 
-# Terminal dependencies
+# CLI dependencies
 prompt-toolkit = "^3.0.16"
 rich = "^13"
 python-dotenv = "^1.0.0"
 openpyxl = "^3.1.2"
 
-[tool.poetry.group.dev.dependencies]
-openbb-devtools = "^1.1.3"
-
 [build-system]
 requires = ["setuptools<65.5.0", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openbb_cli-1.0.0/PKG-INFO` & `openbb_cli-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Investment Research for Everyone, Anywhere.
 Home-page: https://openbb.co
 License: AGPL-3.0-only
 Author: OpenBB
 Author-email: hello@openbb.co
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb[all] (>=4.2.0,<5.0.0)
+Requires-Dist: openbb[all] (>=4.2.1,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.16,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13,<14)
 Project-URL: Documentation, https://docs.openbb.co/terminal
 Project-URL: Repository, https://github.com/OpenBB-finance/OpenBBTerminal
 Description-Content-Type: text/markdown
@@ -29,31 +29,31 @@
 | OpenBB is committed to build the future of investment research by focusing on an open source infrastructure accessible to everyone, everywhere. |
 | :---------------------------------------------------------------------------------------------------------------------------------------------: |
 |              ![OpenBBLogo](https://user-images.githubusercontent.com/25267873/218899768-1f0964b8-326c-4f35-af6f-ea0946ac970b.png)               |
 |                                                 Check our website at [openbb.co](www.openbb.co)                                                 |
 
 ## Overview
 
-The OpenBB CLI is a command line interface that wraps [OpenBB Platform](https://docs.openbb.co/platform).
+The OpenBB Platform CLI is a command line interface that wraps [OpenBB Platform](https://docs.openbb.co/platform).
 
 It offers a convenient way to interact with the OpenBB Platform and its extensions, as well as automate data collection via OpenBB Routine Scripts.
 
-Find the most complete documentation, examples, and usage guides for the OpenBB Platform CLI [here](https://my.openbb.co/app/cli).
+Find the most complete documentation, examples, and usage guides for the OpenBB Platform CLI [here](https://docs.openbb.co/cli).
 
 ## Installation
 
 The command below provides access to the all the available OpenBB extensions behind the OpenBB Platform, find the complete list [here](https://my.openbb.co/app/platform/extensions).
 
 ```bash
 pip install openbb-cli
 ```
 
-> Note: Find the most complete installation hints and tips [here](https://my.openbb.co/app/cli/installation).
+> Note: Find the most complete installation hints and tips [here](https://docs.openbb.co/cli/installation).
 
-After the installation is complete, you can deploy the OpenBB CLI by running the following command:
+After the installation is complete, you can deploy the OpenBB Platform CLI by running the following command:
 
 ```bash
 openbb
 ```
 
 Which should result in the following output:
```

