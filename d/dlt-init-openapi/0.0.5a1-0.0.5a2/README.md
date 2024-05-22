# Comparing `tmp/dlt_init_openapi-0.0.5a1.tar.gz` & `tmp/dlt_init_openapi-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt_init_openapi-0.0.5a1.tar", max compression
+gzip compressed data, was "dlt_init_openapi-0.0.5a2.tar", max compression
```

## Comparing `dlt_init_openapi-0.0.5a1.tar` & `dlt_init_openapi-0.0.5a2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      609 2024-05-21 10:48:17.310114 dlt_init_openapi-0.0.5a1/CHANGELOG.md
--rw-r--r--   0        0        0     1111 2024-05-21 08:48:46.382581 dlt_init_openapi-0.0.5a1/LICENSE
--rw-r--r--   0        0        0     5990 2024-05-21 10:48:17.310708 dlt_init_openapi-0.0.5a1/README.md
--rw-r--r--   0        0        0     4712 2024-05-21 10:48:17.311130 dlt_init_openapi-0.0.5a1/dlt_init_openapi/__init__.py
--rw-r--r--   0        0        0       28 2024-05-21 10:48:17.311493 dlt_init_openapi-0.0.5a1/dlt_init_openapi/__main__.py
--rw-r--r--   0        0        0     3650 2024-05-21 10:48:17.311902 dlt_init_openapi-0.0.5a1/dlt_init_openapi/cli/__init__.py
--rw-r--r--   0        0        0     1151 2024-05-21 10:48:17.312151 dlt_init_openapi-0.0.5a1/dlt_init_openapi/cli/cli_endpoint_selection.py
--rw-r--r--   0        0        0     2908 2024-05-21 10:48:17.312572 dlt_init_openapi-0.0.5a1/dlt_init_openapi/config.py
--rw-r--r--   0        0        0       29 2024-05-21 10:48:17.312788 dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/__init__.py
--rw-r--r--   0        0        0      664 2024-05-21 10:48:17.312992 dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/base_detector.py
--rw-r--r--   0        0        0    22081 2024-05-21 10:48:17.313289 dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/__init__.py
--rw-r--r--   0        0        0     1048 2024-05-21 10:48:17.313587 dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/const.py
--rw-r--r--   0        0        0     1774 2024-05-21 10:48:17.313932 dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/primary_key.py
--rw-r--r--   0        0        0      686 2024-05-21 10:48:17.314162 dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/utils.py
--rw-r--r--   0        0        0     1573 2024-05-21 10:48:17.314794 dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/warnings.py
--rw-r--r--   0        0        0       47 2024-05-21 10:48:17.315112 dlt_init_openapi-0.0.5a1/dlt_init_openapi/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.315259 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/__init__.py
--rw-r--r--   0        0        0       57 2024-05-21 10:48:17.315501 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/config.py
--rw-r--r--   0        0        0       44 2024-05-21 10:48:17.315659 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/const.py
--rw-r--r--   0        0        0     2839 2024-05-21 10:48:17.315866 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/context.py
--rw-r--r--   0        0        0     9440 2024-05-21 10:48:17.316109 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/endpoints.py
--rw-r--r--   0        0        0     1376 2024-05-21 10:48:17.316256 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/errors.py
--rw-r--r--   0        0        0      704 2024-05-21 10:48:17.316445 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/info.py
--rw-r--r--   0        0        0    12896 2024-05-21 10:48:17.316840 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/models.py
--rw-r--r--   0        0        0     3303 2024-05-21 10:48:17.317188 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/openapi_parser.py
--rw-r--r--   0        0        0      670 2024-05-21 10:48:17.317716 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/pagination.py
--rw-r--r--   0        0        0     2766 2024-05-21 10:48:17.318056 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/parameters.py
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.318258 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/properties/__init__.py
--rw-r--r--   0        0        0     2365 2024-05-21 10:48:17.318463 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/properties/converter.py
--rw-r--r--   0        0        0      499 2024-05-21 10:48:17.318652 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/security.py
--rw-r--r--   0        0        0     2360 2024-05-21 10:48:17.318971 dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/types.py
--rw-r--r--   0        0        0       26 2024-05-21 10:48:17.319147 dlt_init_openapi-0.0.5a1/dlt_init_openapi/py.typed
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.319244 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/__init__.py
--rw-r--r--   0        0        0      516 2024-05-21 10:48:17.319570 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/base_renderer.py
--rw-r--r--   0        0        0     5852 2024-05-21 10:48:17.319911 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/__init__.py
--rw-r--r--   0        0        0      682 2024-05-21 10:48:17.320321 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/README.md.j2
--rw-r--r--   0        0        0      502 2024-05-21 10:48:17.320520 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
--rw-r--r--   0        0        0      121 2024-05-21 10:48:17.320741 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
--rw-r--r--   0        0        0      483 2024-05-21 10:48:17.320968 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
--rw-r--r--   0        0        0       11 2024-05-21 10:48:17.321138 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
--rw-r--r--   0        0        0     3576 2024-05-21 10:48:17.321366 dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/source.py.j2
--rw-r--r--   0        0        0      199 2024-05-21 10:48:17.321712 dlt_init_openapi-0.0.5a1/dlt_init_openapi/typing.py
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.321833 dlt_init_openapi-0.0.5a1/dlt_init_openapi/utils/__init__.py
--rw-r--r--   0        0        0     4098 2024-05-21 10:48:17.322081 dlt_init_openapi-0.0.5a1/dlt_init_openapi/utils/misc.py
--rw-r--r--   0        0        0     3851 2024-05-21 10:48:17.322279 dlt_init_openapi-0.0.5a1/dlt_init_openapi/utils/paths.py
--rw-r--r--   0        0        0     1162 2024-05-21 10:48:17.322584 dlt_init_openapi-0.0.5a1/dlt_init_openapi/utils/update_rest_api.py
--rw-r--r--   0        0        0     2525 2024-05-21 11:36:38.624962 dlt_init_openapi-0.0.5a1/pyproject.toml
--rw-r--r--   0        0        0     7576 1970-01-01 00:00:00.000000 dlt_init_openapi-0.0.5a1/PKG-INFO
+-rw-r--r--   0        0        0      840 2024-05-22 13:53:17.730342 dlt_init_openapi-0.0.5a2/CHANGELOG.md
+-rw-r--r--   0        0        0     1111 2024-05-10 11:31:42.794290 dlt_init_openapi-0.0.5a2/LICENSE
+-rw-r--r--   0        0        0     6195 2024-05-22 13:45:51.993375 dlt_init_openapi-0.0.5a2/README.md
+-rw-r--r--   0        0        0     4712 2024-05-21 17:28:54.409899 dlt_init_openapi-0.0.5a2/dlt_init_openapi/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-21 17:28:54.410188 dlt_init_openapi-0.0.5a2/dlt_init_openapi/__main__.py
+-rw-r--r--   0        0        0     4422 2024-05-22 13:45:51.993633 dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/__init__.py
+-rw-r--r--   0        0        0     1151 2024-05-21 17:28:54.410397 dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/cli_endpoint_selection.py
+-rw-r--r--   0        0        0     3320 2024-05-22 13:45:51.993782 dlt_init_openapi-0.0.5a2/dlt_init_openapi/config.py
+-rw-r--r--   0        0        0       29 2024-05-21 17:28:54.410699 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/__init__.py
+-rw-r--r--   0        0        0      664 2024-05-21 17:28:54.410787 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/base_detector.py
+-rw-r--r--   0        0        0    22081 2024-05-21 17:28:54.410925 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-21 17:28:54.411220 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/const.py
+-rw-r--r--   0        0        0     1774 2024-05-21 17:28:54.411298 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/primary_key.py
+-rw-r--r--   0        0        0      686 2024-05-21 17:28:54.411376 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/utils.py
+-rw-r--r--   0        0        0     1573 2024-05-21 17:28:54.411449 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/warnings.py
+-rw-r--r--   0        0        0       47 2024-05-21 17:28:54.411692 dlt_init_openapi-0.0.5a2/dlt_init_openapi/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:28:54.411786 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-21 17:28:54.411874 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/config.py
+-rw-r--r--   0        0        0       44 2024-05-21 17:28:54.412149 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/const.py
+-rw-r--r--   0        0        0     2839 2024-05-21 17:28:54.412231 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/context.py
+-rw-r--r--   0        0        0     9840 2024-05-22 13:45:51.994295 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/endpoints.py
+-rw-r--r--   0        0        0     1376 2024-05-21 17:28:54.412635 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/errors.py
+-rw-r--r--   0        0        0      704 2024-05-21 17:28:54.412728 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/info.py
+-rw-r--r--   0        0        0    12896 2024-05-21 17:28:54.412851 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/models.py
+-rw-r--r--   0        0        0     3303 2024-05-21 17:28:54.412942 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/openapi_parser.py
+-rw-r--r--   0        0        0      670 2024-05-21 17:28:54.413023 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/pagination.py
+-rw-r--r--   0        0        0     2766 2024-05-21 17:28:54.413107 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/parameters.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:28:54.413182 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/properties/__init__.py
+-rw-r--r--   0        0        0     2365 2024-05-21 17:28:54.413458 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/properties/converter.py
+-rw-r--r--   0        0        0      499 2024-05-21 17:28:54.413846 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/security.py
+-rw-r--r--   0        0        0     2360 2024-05-21 17:28:54.413941 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/types.py
+-rw-r--r--   0        0        0       26 2024-05-21 17:28:54.414020 dlt_init_openapi-0.0.5a2/dlt_init_openapi/py.typed
+-rw-r--r--   0        0        0        0 2024-05-21 17:28:54.414102 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-21 17:28:54.414198 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/base_renderer.py
+-rw-r--r--   0        0        0     5869 2024-05-22 13:45:51.994512 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-21 17:28:54.414420 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/README.md.j2
+-rw-r--r--   0        0        0      519 2024-05-22 13:45:51.994842 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
+-rw-r--r--   0        0        0      148 2024-05-22 13:45:51.995003 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
+-rw-r--r--   0        0        0      479 2024-05-22 13:45:51.995143 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
+-rw-r--r--   0        0        0       11 2024-05-21 17:28:54.415547 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
+-rw-r--r--   0        0        0     3774 2024-05-22 13:45:51.995284 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/source.py.j2
+-rw-r--r--   0        0        0      199 2024-05-21 17:28:54.415943 dlt_init_openapi-0.0.5a2/dlt_init_openapi/typing.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:28:54.416023 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/__init__.py
+-rw-r--r--   0        0        0     4137 2024-05-22 13:45:51.995498 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/misc.py
+-rw-r--r--   0        0        0     3851 2024-05-21 17:28:54.416842 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/paths.py
+-rw-r--r--   0        0        0     1162 2024-05-21 17:28:54.416919 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/update_rest_api.py
+-rw-r--r--   0        0        0     2536 2024-05-22 13:53:17.730687 dlt_init_openapi-0.0.5a2/pyproject.toml
+-rw-r--r--   0        0        0     7781 1970-01-01 00:00:00.000000 dlt_init_openapi-0.0.5a2/PKG-INFO
```

### Comparing `dlt_init_openapi-0.0.5a1/LICENSE` & `dlt_init_openapi-0.0.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/README.md` & `dlt_init_openapi-0.0.5a2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -122,10 +122,13 @@
 
 And use it with the config argument:
 
 ```console
 $ dlt-init-openapi init pokemon --url ... --config config.yml
 ```
 
+## Telemetry
+We track your usage of this tool similar to how we track other commands in the dlt core library. Read more about this and how to disable it here: https://dlthub.com/docs/reference/telemetry.
+
 ## Implementation notes
 * OAuth Authentication currently is not natively supported, you can supply your own
 * Per endpoint authentication currently is not supported by the generator, only the first globally set securityScheme will be applied. You can add your own per endpoint if you need to.
```

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/__init__.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/cli/__init__.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pathlib
 import sys
 from typing import Any, Optional
 
 import questionary
 import typer
+from dlt.cli import utils
 from loguru import logger
 
 from dlt_init_openapi.cli.cli_endpoint_selection import questionary_endpoint_selection
 from dlt_init_openapi.config import Config
 from dlt_init_openapi.utils import update_rest_api
 
-app = typer.Typer()
+app = typer.Typer(add_completion=False)
 
 
 def _print_version(value: bool) -> None:
     from dlt_init_openapi import __version__
 
     if value:
         typer.echo(f"dlt-init-openapi version: {__version__}")
@@ -56,14 +57,40 @@
     loglevel: int = typer.Option(20, help="Set logging level for stdout output, defaults to 20 (INFO)"),
     global_limit: int = typer.Option(0, help="Set a global limit on the generated source"),
     update_rest_api_source: bool = typer.Option(
         False, help="Wether to update the locally cached rest_api verified source"
     ),
 ) -> None:
     """Generate a new OpenAPI Client library"""
+    _init_command_wrapped(
+        source=source,
+        url=url,
+        path=path,
+        output_path=output_path,
+        config_path=config_path,
+        interactive=interactive,
+        loglevel=loglevel,
+        global_limit=global_limit,
+        update_rest_api_source=update_rest_api_source,
+    )
+
+
+@utils.track_command("init-openapi", False, "source", "url", "path")
+def _init_command_wrapped(
+    source: str,
+    url: Optional[str] = None,
+    path: Optional[pathlib.Path] = None,
+    output_path: Optional[pathlib.Path] = None,
+    config_path: Optional[pathlib.Path] = None,
+    interactive: bool = True,
+    loglevel: int = 20,
+    global_limit: int = 0,
+    update_rest_api_source: bool = False,
+) -> None:
+
     from dlt_init_openapi import create_new_client
 
     # set up console logging
     logger.remove()
     logger.add(sys.stdout, level=loglevel)
     logger.success("Starting dlt openapi generator")
```

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/cli/cli_endpoint_selection.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/cli_endpoint_selection.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/config.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import pathlib
 from pathlib import Path
 from typing import Any, List, Optional
 
 import yaml
 from pydantic import BaseModel
 
+from dlt_init_openapi.utils.misc import snake_case
+
 from .typing import TEndpointFilter
 
 REST_API_SOURCE_LOCATION = str(pathlib.Path(__file__).parent.resolve() / "../rest_api")
 
 
 class Config(BaseModel):
     """Contains any configurable values passed by the user."""
@@ -27,16 +29,18 @@
         "black .",
     ]
     """Commands to run after code generation"""
     include_methods: List[str] = ["get"]
     """HTTP methods to render from OpenAPI spec"""
     fallback_openapi_title: str = "openapi"
     """Fallback title when openapi info.title is missing or empty"""
-    project_folder_suffix: str = "-pipeline"
+    project_folder_suffix: str = "_pipeline"
     """Suffix for project name"""
+    pipeline_file_suffix: str = "_pipeline.py"
+    """Suffix for pipeline file name"""
     dataset_name_suffix: str = "_data"
     """Suffix for dataset"""
     endpoint_filter: Optional[TEndpointFilter] = None
     """filter for endpoint rendering"""
     name_resources_by_operation: bool = False
     """always name resources by operation id, useful for testing"""
     renderer_class: str = "dlt_init_openapi.renderer.default.DefaultRenderer"
@@ -46,24 +50,30 @@
     global_limit: int = 0
     """Set a limit on how many items are emitted from a resource"""
     parameter_default_value: str = "FILL_ME_IN"
     """default to render for required parameters that do not have a default in the spec"""
 
     # internal, do not set via config file
     project_dir: Path = None
+    pipeline_file_name: str = None
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Config, self).__init__(*args, **kwargs)
         self.prepare()
 
     def prepare(self) -> None:
+        # normalize a couple of vars
+        self.project_name = snake_case(self.project_name)
+        self.package_name = snake_case(self.package_name)
+
         if self.project_name and self.project_folder_suffix:
             base_dir = Path.cwd() if not self.output_path else Path.cwd() / self.output_path
             project_folder = self.project_name + self.project_folder_suffix
             self.project_dir = base_dir / project_folder
+            self.pipeline_file_name = self.project_name + self.pipeline_file_suffix
 
     @staticmethod
     def load_from_path(path: Path, *args: Any, **kwargs: Any) -> "Config":
         """Creates a Config from provided JSON or YAML file and sets a bunch of globals from it"""
         mime = mimetypes.guess_type(path.absolute().as_uri(), strict=True)[0]
         if mime == "application/json":
             config_data = json.loads(path.read_text())
```

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/base_detector.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/base_detector.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/__init__.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/const.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/const.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/primary_key.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/primary_key.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/utils.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/utils.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/detector/default/warnings.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/context.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/context.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/endpoints.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,25 @@
     def render_pagination_args(self) -> Optional[Dict[str, Union[str, int]]]:
         # if own paginator equals global paginator, do not render anything
         if self.detected_pagination == self.detected_global_pagination:
             return None
         return self.detected_pagination.paginator_config if self.detected_pagination else None
 
     @property
+    def render_auto_paginator(self) -> bool:
+        """if we could not figure out the paginator, set it to auto"""
+        # we do not set auto if there is a global paginator, this is a bug in the underlying layer, we have to fix this
+        # once rest_api is fixed
+        if self.detected_global_pagination:
+            return False
+        return not (self.detected_pagination)
+
+    @property
     def data_json_path(self) -> str:
-        return self.payload.json_path if self.payload else "$"
+        return self.payload.json_path if self.payload else None
 
     @property
     def transformer(self) -> Optional[TransformerSetting]:
         return self.detected_transformer_settings
 
     @property
     def unresolvable_path_param_names(self) -> List[str]:
```

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/errors.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/errors.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/info.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/info.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/models.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/models.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/openapi_parser.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/openapi_parser.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/pagination.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/pagination.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/parameters.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/parameters.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/properties/converter.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/properties/converter.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/parser/types.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/types.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/base_renderer.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/base_renderer.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/__init__.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 self.openapi.detected_global_pagination.paginator_config
                 if self.openapi.detected_global_pagination
                 else None
             ),
         )
 
     def _build_pipeline(self) -> None:
-        module_path = self.config.project_dir / "pipeline.py"
+        module_path = self.config.project_dir / self.config.pipeline_file_name
 
         template = self.env.get_template("pipeline.py.j2")
         module_path.write_text(
             template.render(
                 package_name=self.package_name,
                 source_name=self.source_name,
                 dataset_name=self.dataset_name,
```

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/README.md.j2` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/renderer/default/templates/source.py.j2` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/source.py.j2`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,17 @@
             "primary_key": "{{ endpoint.primary_key }}",
             "write_disposition": "merge",
             {% if endpoint.id in endpoint_collection.endpoint_ids_to_deselect %}
             "selected": False,
             {% endif %}
             {% endif %}
             "endpoint": {
+                {% if endpoint.data_json_path %}
                 "data_selector": "{{ endpoint.data_json_path }}",
+                {% endif %}
                 "path": "{{endpoint.path }}",
                 {% if endpoint.transformer or endpoint.unresolvable_path_param_names or endpoint.unresolvable_query_param_names %}
                 "params": {
                     {% if endpoint.transformer %}
                     {% for key, value in endpoint.transformer.path_params_mapping.items()%}
                     "{{key}}": {
                         "type": "resolve",
@@ -80,14 +82,17 @@
                         {{value}},
                         {% else %}
                         "{{value}}",
                         {% endif %}
                     {% endfor %}
                 },
                 {% endif %}
+                {% if endpoint.render_auto_paginator %}
+                "paginator": "auto",
+                {% endif %}
             }
         },
         {% endfor %}
         ]
     }
 
     return rest_api_source(source_config)
```

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/utils/misc.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     if value in RESERVED_WORDS or iskeyword(value):
         return f"{value}_"
     return value
 
 
 def snake_case(value: str) -> str:
     """Converts to snake_case"""
+    if not value:
+        return value
     words = split_words(sanitize(value))
     return "_".join(words).lower()
 
 
 def pascal_case(value: str) -> str:
     """Converts to PascalCase"""
     words = split_words(sanitize(value))
```

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/utils/paths.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/paths.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/dlt_init_openapi/utils/update_rest_api.py` & `dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/update_rest_api.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a1/pyproject.toml` & `dlt_init_openapi-0.0.5a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt-init-openapi"
-version = "0.0.5a1"
+version = "0.0.5a2"
 description = "Generate dlt Python clients from OpenAPI"
 homepage = "https://dlthub.com"
 repository = "https://github.com/dlt-hub/dlt-init-openapi"
 license = "MIT"
 keywords=["OpenAPI", "Client", "Generator"]
 authors = ["David Scharf <david@dlthub.com>"]
 classifiers = [
@@ -40,16 +40,16 @@
 loguru = "^0.7.2"
 
 [tool.poetry.scripts]
 dlt-init-openapi = "dlt_init_openapi.cli:app"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
-pytest = "*"
-pytest-mock = "*"
+pytest = "^7.0.0"
+pytest-mock = "^3.14.0"
 mypy = "*"
 pytest-cov = "*"
 python-multipart = "*"
 types-PyYAML = "^6.0.3"
 types-certifi = "^2020.0.0"
 types-python-dateutil = "^2.0.0"
 types-requests = "^2.31.0.20240406"
```

### Comparing `dlt_init_openapi-0.0.5a1/PKG-INFO` & `dlt_init_openapi-0.0.5a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt-init-openapi
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: Generate dlt Python clients from OpenAPI
 Home-page: https://dlthub.com
 License: MIT
 Keywords: OpenAPI,Client,Generator
 Author: David Scharf
 Author-email: david@dlthub.com
 Requires-Python: >=3.9,<3.13
@@ -162,11 +162,14 @@
 
 And use it with the config argument:
 
 ```console
 $ dlt-init-openapi init pokemon --url ... --config config.yml
 ```
 
+## Telemetry
+We track your usage of this tool similar to how we track other commands in the dlt core library. Read more about this and how to disable it here: https://dlthub.com/docs/reference/telemetry.
+
 ## Implementation notes
 * OAuth Authentication currently is not natively supported, you can supply your own
 * Per endpoint authentication currently is not supported by the generator, only the first globally set securityScheme will be applied. You can add your own per endpoint if you need to.
```

