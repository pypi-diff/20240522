# Comparing `tmp/py_allspice-3.0.0.tar.gz` & `tmp/py_allspice-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_allspice-3.0.0.tar", last modified: Fri May 10 14:34:57 2024, max compression
+gzip compressed data, was "py_allspice-3.1.0.tar", last modified: Tue May 21 23:48:32 2024, max compression
```

## Comparing `py_allspice-3.0.0.tar` & `py_allspice-3.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.861518 py_allspice-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 14:34:50.000000 py_allspice-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-10 14:34:57.857518 py_allspice-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-10 14:34:50.000000 py_allspice-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/allspice/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/allspice.py
--rw-r--r--   0 runner    (1001) docker     (127)    75142 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/apiobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/baseapiobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/ratelimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/allspice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21370 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/bom_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-10 14:34:50.000000 py_allspice-3.0.0/allspice/utils/netlist_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/py_allspice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 14:34:57.000000 py_allspice-3.0.0/py_allspice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 14:34:50.000000 py_allspice-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:34:57.861518 py_allspice-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-10 14:34:50.000000 py_allspice-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:34:57.857518 py_allspice-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    32675 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_api_longtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_api_ratelimiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-10 14:34:50.000000 py_allspice-3.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:48:32.778411 py_allspice-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 23:48:28.000000 py_allspice-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-21 23:48:32.778411 py_allspice-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-21 23:48:28.000000 py_allspice-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:48:32.774411 py_allspice-3.1.0/allspice/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/allspice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75142 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/apiobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/baseapiobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/ratelimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:48:32.774411 py_allspice-3.1.0/allspice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27059 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/utils/bom_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/utils/list_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-21 23:48:28.000000 py_allspice-3.1.0/allspice/utils/netlist_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:48:32.778411 py_allspice-3.1.0/py_allspice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-21 23:48:32.000000 py_allspice-3.1.0/py_allspice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-21 23:48:32.000000 py_allspice-3.1.0/py_allspice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:48:32.000000 py_allspice-3.1.0/py_allspice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 23:48:32.000000 py_allspice-3.1.0/py_allspice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 23:48:32.000000 py_allspice-3.1.0/py_allspice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 23:48:28.000000 py_allspice-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:48:32.778411 py_allspice-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-21 23:48:28.000000 py_allspice-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:48:32.778411 py_allspice-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    32675 2024-05-21 23:48:28.000000 py_allspice-3.1.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-21 23:48:28.000000 py_allspice-3.1.0/tests/test_api_longtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-21 23:48:28.000000 py_allspice-3.1.0/tests/test_api_ratelimiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-21 23:48:28.000000 py_allspice-3.1.0/tests/test_utils.py
```

### Comparing `py_allspice-3.0.0/LICENSE` & `py_allspice-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/PKG-INFO` & `py_allspice-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 3.0.0
+Version: 3.1.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/AllSpiceIO/py-allspice
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py_allspice-3.0.0/README.md` & `py_allspice-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/allspice/allspice.py` & `py_allspice-3.1.0/allspice/allspice.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/allspice/apiobject.py` & `py_allspice-3.1.0/allspice/apiobject.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/allspice/baseapiobject.py` & `py_allspice-3.1.0/allspice/baseapiobject.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/allspice/exceptions.py` & `py_allspice-3.1.0/allspice/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/allspice/ratelimiter.py` & `py_allspice-3.1.0/allspice/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/allspice/utils/bom_generation.py` & `py_allspice-3.1.0/allspice/utils/bom_generation.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from enum import Enum
 from logging import Logger
 import pathlib
 import re
 import time
 from typing import Optional, Union
 
+from .list_components import list_components_for_orcad
+
 from ..allspice import AllSpice
 from ..apiobject import Ref, Repository
 from ..exceptions import NotYetGeneratedException
 
 REPETITIONS_REGEX = re.compile(r"Repeat\(\w+,(\d+),(\d+)\)")
 QUANTITY_COLUMN_NAME = "Quantity"
 DESIGNATOR_COLUMN_NAME = "Designator"
@@ -30,31 +32,113 @@
 # the number of repetitions of that child sheet in the parent sheet.
 SchdocHierarchy = dict[str, list[tuple[str, int]]]
 ComponentAttributes = dict[str, str | None]
 BomEntry = dict[str, str]
 Bom = list[BomEntry]
 
 
+def generate_bom(
+    allspice_client: AllSpice,
+    repository: Repository,
+    source_file: str,
+    columns: ColumnsMapping,
+    group_by: Optional[list[str]] = None,
+    variant: Optional[str] = None,
+    ref: Ref = "main",
+) -> Bom:
+    """
+    Generate a BOM for a project.
+
+    :param allspice_client: The AllSpice client to use.
+    :param repository: The repository to generate the BOM for.
+    :param source_file: The path to the source file from the root of the
+        repository. The source file must be a PrjPcb file for Altium projects
+        and a DSN file for OrCAD projects. For example, if the source file is
+        in the root of the repository and is named "Archimajor.PrjPcb", the
+        path would be "Archimajor.PrjPcb"; if the source file is in a folder
+        called "Schematics" and is named "Beagleplay.dsn", the path would be
+        "Schematics/Beagleplay.dsn".
+    :param columns: A mapping of the columns in the BOM to the attributes in the
+        project. The attributes are tried in order, and the first one found is
+        used as the value for that column.
+
+        For example, if there should be a "Part Number" column in the BOM, and
+        the value for that column can be in the "Part" or "MFN Part#" attributes
+        in the project, the following mapping can be used:
+
+                {
+                    "Part Number": ["Part", "MFN Part#"]
+                }
+
+        In this case, the "Part" attribute will be checked first, and if it is
+        not present, the "MFN Part#" attribute will be checked. If neither are
+        present, the "Part Number" column in the BOM will be empty.
+    :param group_by: A list of columns to group the BOM by. If this is provided,
+        the BOM will be grouped by the values of these columns.
+    :param variant: The variant of the project to generate the BOM for. If this
+        is provided, the BOM will be generated for the specified variant. If
+        this is not provided, or is None, the BOM will be generated for the
+        default variant. Variants are not supported for OrCAD projects.
+    :param ref: The ref, i.e. branch, commit or git ref from which to take the
+        project files. Defaults to "main".
+    :return: A list of BOM entries. Each entry is a dictionary where the key is
+        a column name and the value is the value for that column.
+    """
+
+    if source_file.lower().endswith(".prjpcb"):
+        project_tool = "altium"
+    elif source_file.lower().endswith(".dsn"):
+        project_tool = "orcad"
+    else:
+        raise ValueError(
+            "The source file must be a PrjPcb file for Altium projects or a DSN file for OrCAD "
+            "projects."
+        )
+
+    match project_tool:
+        case "altium":
+            return generate_bom_for_altium(
+                allspice_client,
+                repository,
+                source_file,
+                columns,
+                group_by,
+                variant,
+                ref,
+            )
+        case "orcad":
+            if variant:
+                raise ValueError("Variant is not supported for OrCAD projects.")
+
+            return generate_bom_for_orcad(
+                allspice_client,
+                repository,
+                source_file,
+                columns,
+                group_by,
+                ref,
+            )
+
+
 def generate_bom_for_altium(
     allspice_client: AllSpice,
     repository: Repository,
     prjpcb_file: str,
     columns: ColumnsMapping,
     group_by: Optional[list[str]] = None,
     variant: Optional[str] = None,
     ref: Ref = "main",
 ) -> Bom:
     """
     Generate a BOM for an Altium project.
 
     :param allspice_client: The AllSpice client to use.
     :param repository: The repository to generate the BOM for.
-    :param prjpcb_file: The Altium project file. This can be a Content object
-        returned by the AllSpice API, or a string containing the path to the
-        file in the repo.
+    :param prjpcb_file: The path to the PrjPcb project file from the root of the
+        repository.
     :param columns: A mapping of the columns in the BOM to the attributes in the
         Altium project. The attributes are tried in order, and the first one
         found is used as the value for that column.
 
         For example, if there  should be a "Part Number" column in the BOM, and
         the value for that column can be in the "Part" or "MFN Part#" attributes
         in the Altium project, the following mapping can be used:
@@ -141,14 +225,67 @@
 
     mapped_components = _map_attributes(components, columns)
     bom = _group_entries(mapped_components, group_by)
 
     return bom
 
 
+def generate_bom_for_orcad(
+    allspice_client: AllSpice,
+    repository: Repository,
+    dsn_path: str,
+    columns: ColumnsMapping,
+    group_by: Optional[list[str]] = None,
+    ref: Ref = "main",
+) -> Bom:
+    """
+    Generate a BOM for an OrCAD schematic.
+
+    :param allspice_client: The AllSpice client to use.
+    :param repository: The repository to generate the BOM for.
+    :param dsn_path: The OrCAD DSN file. This can be a Content object returned
+        by the AllSpice API, or a string containing the path to the file in the
+        repo.
+    :param columns: A mapping of the columns in the BOM to the attributes in the
+        OrCAD schematic. The attributes are tried in order, and the first one
+        found is used as the value for that column.
+
+        For example, if there  should be a "Part Number" column in the BOM, and
+        the value for that column can be in the "Part" or "MFN Part#" attributes
+        in the OrCAD schematic, the following mapping can be used:
+
+            {
+                "Part Number": ["Part", "MFN Part#"]
+            }
+
+        In this case, the "Part" attribute will be checked first, and if it is
+        not present, the "MFN Part#" attribute will be checked. If neither are
+        present, the "Part Number" column in the BOM will be empty.
+    :param group_by: A list of columns to group the BOM by. If this is provided,
+        the BOM will be grouped by the values of these columns.
+    :param ref: The ref, i.e. branch, commit or git ref from which to take the
+        project files. Defaults to "main".
+    :return: A list of BOM entries. Each entry is a dictionary where the key is
+        a column name and the value is the value for that column.
+    """
+
+    allspice_client.logger.debug(
+        f"Generating BOM for {repository.get_full_name()=} on {ref=} using {columns=}"
+    )
+    if group_by is not None:
+        for group_column in group_by:
+            if group_column not in columns:
+                raise ValueError(f"Group by column {group_column} not found in selected columns")
+    components = list_components_for_orcad(allspice_client, repository, dsn_path, ref)
+    mapped_components = _map_attributes(components, columns)
+    bom = _group_entries(mapped_components, group_by)
+
+    return bom
+
+
 def _get_first_matching_key_value(
     alternatives: Union[list[str], str],
     attributes: dict[str, str | None],
 ) -> Optional[str]:
     """
     Search for a series of alternative keys in a dictionary, and return the
     value of the first one found.
@@ -187,14 +324,16 @@
     # PrjPcb path (which is a Posix Path, since it is from ASH), and then
     # convert the result into a posix path as a string for use in ASH.
     schdoc = pathlib.PureWindowsPath(schdoc_path)
     prjpcb = pathlib.PurePosixPath(prjpcb_path)
     return (prjpcb.parent / schdoc).as_posix()
 
 
+# TODO: Remove this after altium component listing has been refactored to
+#   list_components.py.
 def _fetch_generated_json(repo: Repository, file_path: str, ref: Ref, logger: Logger) -> dict:
     attempts = 0
     while attempts < 5:
         try:
             return repo.get_generated_json(file_path, ref=ref)
         except NotYetGeneratedException:
             logger.info(f"JSON for {file_path} is not yet generated. Retrying in 0.5s.")
```

### Comparing `py_allspice-3.0.0/allspice/utils/core.py` & `py_allspice-3.1.0/allspice/utils/core.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/allspice/utils/netlist_generation.py` & `py_allspice-3.1.0/allspice/utils/netlist_generation.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/py_allspice.egg-info/PKG-INFO` & `py_allspice-3.1.0/py_allspice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 3.0.0
+Version: 3.1.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/AllSpiceIO/py-allspice
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py_allspice-3.0.0/py_allspice.egg-info/SOURCES.txt` & `py_allspice-3.1.0/py_allspice.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 allspice/apiobject.py
 allspice/baseapiobject.py
 allspice/exceptions.py
 allspice/ratelimiter.py
 allspice/utils/__init__.py
 allspice/utils/bom_generation.py
 allspice/utils/core.py
+allspice/utils/list_components.py
 allspice/utils/netlist_generation.py
 py_allspice.egg-info/PKG-INFO
 py_allspice.egg-info/SOURCES.txt
 py_allspice.egg-info/dependency_links.txt
 py_allspice.egg-info/requires.txt
 py_allspice.egg-info/top_level.txt
 tests/test_api.py
```

### Comparing `py_allspice-3.0.0/tests/test_api.py` & `py_allspice-3.1.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/tests/test_api_longtests.py` & `py_allspice-3.1.0/tests/test_api_longtests.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/tests/test_api_ratelimiting.py` & `py_allspice-3.1.0/tests/test_api_ratelimiting.py`

 * *Files identical despite different names*

### Comparing `py_allspice-3.0.0/tests/test_utils.py` & `py_allspice-3.1.0/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import base64
 import csv
+import json
 import uuid
 
 import pytest
 
 from allspice import AllSpice
-from allspice.utils.bom_generation import generate_bom_for_altium
+from allspice.utils.bom_generation import (
+    generate_bom,
+    generate_bom_for_altium,
+    generate_bom_for_orcad,
+)
+from allspice.utils.list_components import list_components_for_orcad
 from allspice.utils.netlist_generation import generate_netlist
 
 test_repo = "repo_" + uuid.uuid4().hex[:8]
 test_branch = "branch_" + uuid.uuid4().hex[:8]
 
 
 @pytest.fixture(scope="session")
@@ -303,14 +309,132 @@
 
     with open("tests/data/archimajor_bom_fitted_grouped_expected.csv", "r") as f:
         reader = csv.DictReader(f)
         for row, expected_row in zip(reader, bom):
             assert row == expected_row
 
 
+def test_bom_generation_orcad(request, instance):
+    _setup_for_generation(
+        instance,
+        request.node.name,
+        "https://hub.allspice.io/AllSpiceMirrors/beagleplay.git",
+    )
+    repo = instance.get_repository(
+        instance.get_user().username, "-".join([test_repo, request.node.name])
+    )
+    attributes_mapping = {
+        "Name": ["_name"],
+        "Description": "Description",
+        "Reference designator": ["Part Reference"],
+        "Manufacturer": ["Manufacturer", "MANUFACTURER"],
+        "Part Number": ["Manufacturer PN", "PN"],
+    }
+
+    bom = generate_bom_for_orcad(
+        instance,
+        repo,
+        "Design/BEAGLEPLAYV10_221227.DSN",
+        attributes_mapping,
+        # We hard-code a ref so that this test is reproducible.
+        ref="7a59a98ae27dc4fd9e2bd8975ff90cdb44a366ea",
+    )
+
+    assert len(bom) == 870
+
+    with open("tests/data/beagleplay_bom_expected.csv", "r") as f:
+        reader = csv.DictReader(f)
+        for row, expected_row in zip(reader, bom):
+            assert row == expected_row
+
+
+def test_generate_bom(request, instance):
+    # Test the one-stop API which should automatically figure out the project
+    # type and call the appropriate function.
+    _setup_for_generation(
+        instance,
+        request.node.name + "altium",
+        "https://hub.allspice.io/ProductDevelopmentFirm/ArchimajorDemo.git",
+    )
+    _setup_for_generation(
+        instance,
+        request.node.name + "orcad",
+        "https://hub.allspice.io/AllSpiceMirrors/beagleplay.git",
+    )
+
+    repo = instance.get_repository(
+        instance.get_user().username, "-".join([test_repo, request.node.name + "altium"])
+    )
+    altium_attributes_mapping = {
+        "description": ["PART DESCRIPTION"],
+        "designator": ["Designator"],
+        "manufacturer": ["Manufacturer", "MANUFACTURER"],
+        "part_number": ["PART", "MANUFACTURER #"],
+    }
+    bom = generate_bom(
+        instance,
+        repo,
+        "Archimajor.PrjPcb",
+        altium_attributes_mapping,
+        ref="95719adde8107958bf40467ee092c45b6ddaba00",
+    )
+    assert len(bom) == 1061
+    with open("tests/data/archimajor_bom_flat_expected.csv", "r") as f:
+        reader = csv.DictReader(f)
+        for row, expected_row in zip(reader, bom):
+            assert row == expected_row
+
+    repo = instance.get_repository(
+        instance.get_user().username, "-".join([test_repo, request.node.name + "orcad"])
+    )
+    orcad_attributes_mapping = {
+        "Name": ["_name"],
+        "Description": "Description",
+        "Reference designator": ["Part Reference"],
+        "Manufacturer": ["Manufacturer", "MANUFACTURER"],
+        "Part Number": ["Manufacturer PN", "PN"],
+    }
+    bom = generate_bom(
+        instance,
+        repo,
+        "Design/BEAGLEPLAYV10_221227.DSN",
+        orcad_attributes_mapping,
+        ref="7a59a98ae27dc4fd9e2bd8975ff90cdb44a366ea",
+    )
+    assert len(bom) == 870
+    with open("tests/data/beagleplay_bom_expected.csv", "r") as f:
+        reader = csv.DictReader(f)
+        for row, expected_row in zip(reader, bom):
+            assert row == expected_row
+
+
+def test_orcad_components_list(request, instance):
+    _setup_for_generation(
+        instance,
+        request.node.name,
+        "https://hub.allspice.io/AllSpiceMirrors/beagleplay.git",
+    )
+    repo = instance.get_repository(
+        instance.get_user().username, "-".join([test_repo, request.node.name])
+    )
+
+    components = list_components_for_orcad(
+        instance,
+        repo,
+        "Design/BEAGLEPLAYV10_221227.DSN",
+        # We hard-code a ref so that this test is reproducible.
+        ref="7a59a98ae27dc4fd9e2bd8975ff90cdb44a366ea",
+    )
+
+    assert len(components) == 870
+
+    with open("tests/data/beagleplay_components_expected.json", "r") as f:
+        assert json.loads(f.read()) == components
+
+
 def test_netlist_generation(request, instance):
     _setup_for_generation(
         instance,
         request.node.name,
         "https://hub.allspice.io/ProductDevelopmentFirm/ArchimajorDemo.git",
     )
     repo = instance.get_repository(
```

