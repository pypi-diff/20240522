# Comparing `tmp/remotivelabs_cli-0.0.8.tar.gz` & `tmp/remotivelabs_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.8.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.9.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.8.tar` & `remotivelabs_cli-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      608 2023-07-25 06:18:17.909231 remotivelabs_cli-0.0.8/LICENSE
--rw-r--r--   0        0        0      278 2024-02-21 11:33:54.345406 remotivelabs_cli-0.0.8/README.md
--rw-r--r--   0        0        0      122 2024-02-26 09:32:34.929571 remotivelabs_cli-0.0.8/cli/__about__.py
--rw-r--r--   0        0        0        0 2024-02-26 09:32:34.929678 remotivelabs_cli-0.0.8/cli/__init__.py
--rw-r--r--   0        0        0     5338 2024-02-28 09:16:52.363275 remotivelabs_cli-0.0.8/cli/broker/brokers.py
--rw-r--r--   0        0        0     3773 2024-02-28 09:16:52.364011 remotivelabs_cli-0.0.8/cli/broker/export.py
--rw-r--r--   0        0        0     4133 2024-02-28 09:16:52.364333 remotivelabs_cli-0.0.8/cli/broker/files.py
--rw-r--r--   0        0        0      141 2024-02-26 09:32:34.931326 remotivelabs_cli-0.0.8/cli/broker/lib/__about__.py
--rw-r--r--   0        0        0    19711 2024-02-28 12:10:07.869540 remotivelabs_cli-0.0.8/cli/broker/lib/broker.py
--rw-r--r--   0        0        0     1319 2024-02-26 09:32:34.932050 remotivelabs_cli-0.0.8/cli/broker/lib/errors.py
--rw-r--r--   0        0        0     4846 2024-02-28 09:16:52.365096 remotivelabs_cli-0.0.8/cli/broker/playback.py
--rw-r--r--   0        0        0     1382 2024-02-28 09:16:52.366084 remotivelabs_cli-0.0.8/cli/broker/record.py
--rw-r--r--   0        0        0     2896 2024-02-28 12:10:07.863119 remotivelabs_cli-0.0.8/cli/broker/scripting.py
--rw-r--r--   0        0        0     6771 2024-02-28 12:10:07.863491 remotivelabs_cli-0.0.8/cli/broker/signals.py
--rw-r--r--   0        0        0        1 2023-07-25 06:18:17.910408 remotivelabs_cli-0.0.8/cli/cloud/__init__.py
--rw-r--r--   0        0        0     3470 2024-02-28 12:15:04.139940 remotivelabs_cli-0.0.8/cli/cloud/auth.py
--rw-r--r--   0        0        0     3408 2024-02-28 09:16:52.367267 remotivelabs_cli-0.0.8/cli/cloud/auth_tokens.py
--rw-r--r--   0        0        0     4127 2024-02-28 09:16:52.367702 remotivelabs_cli-0.0.8/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1443 2024-02-28 09:16:52.367911 remotivelabs_cli-0.0.8/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3489 2024-02-28 09:16:52.368159 remotivelabs_cli-0.0.8/cli/cloud/configs.py
--rw-r--r--   0        0        0     1369 2024-02-28 09:16:52.368526 remotivelabs_cli-0.0.8/cli/cloud/projects.py
--rw-r--r--   0        0        0    19602 2024-02-28 09:16:52.368715 remotivelabs_cli-0.0.8/cli/cloud/recordings.py
--rw-r--r--   0        0        0     5885 2024-02-28 09:16:52.368931 remotivelabs_cli-0.0.8/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0      639 2024-02-28 09:16:52.369121 remotivelabs_cli-0.0.8/cli/cloud/sample_recordings.py
--rw-r--r--   0        0        0     2294 2024-02-28 09:16:52.369341 remotivelabs_cli-0.0.8/cli/cloud/service_account_tokens.py
--rw-r--r--   0        0        0     1606 2024-02-28 09:16:52.369624 remotivelabs_cli-0.0.8/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0        1 2024-02-01 07:14:42.165748 remotivelabs_cli-0.0.8/cli/connect/__init__.py
--rw-r--r--   0        0        0      927 2024-02-28 09:16:52.370124 remotivelabs_cli-0.0.8/cli/connect/connect.py
--rw-r--r--   0        0        0     3869 2024-02-26 09:32:34.937441 remotivelabs_cli-0.0.8/cli/connect/protopie/protopie.py
--rw-r--r--   0        0        0     1645 2024-02-28 09:16:52.370543 remotivelabs_cli-0.0.8/cli/remotive.py
--rw-r--r--   0        0        0       78 2023-09-06 06:52:38.303129 remotivelabs_cli-0.0.8/cli/requirements.txt
--rw-r--r--   0        0        0      792 2024-02-26 09:32:34.938003 remotivelabs_cli-0.0.8/cli/settings.py
--rw-r--r--   0        0        0        1 2023-12-20 19:10:34.752361 remotivelabs_cli-0.0.8/cli/tools/__init__.py
--rw-r--r--   0        0        0        1 2023-12-20 19:10:34.752447 remotivelabs_cli-0.0.8/cli/tools/can/__init__.py
--rw-r--r--   0        0        0     2407 2024-02-28 09:16:52.371158 remotivelabs_cli-0.0.8/cli/tools/can/can.py
--rw-r--r--   0        0        0      198 2023-12-20 19:10:34.752839 remotivelabs_cli-0.0.8/cli/tools/tools.py
--rw-r--r--   0        0        0      637 2024-02-28 12:29:15.397297 remotivelabs_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      608 2023-07-25 06:18:17.909231 remotivelabs_cli-0.0.9/LICENSE
+-rw-r--r--   0        0        0      278 2024-02-21 11:33:54.345406 remotivelabs_cli-0.0.9/README.md
+-rw-r--r--   0        0        0      122 2024-02-26 09:32:34.929571 remotivelabs_cli-0.0.9/cli/__about__.py
+-rw-r--r--   0        0        0        0 2024-02-26 09:32:34.929678 remotivelabs_cli-0.0.9/cli/__init__.py
+-rw-r--r--   0        0        0     5338 2024-02-28 09:16:52.363275 remotivelabs_cli-0.0.9/cli/broker/brokers.py
+-rw-r--r--   0        0        0     3734 2024-03-12 09:33:52.747712 remotivelabs_cli-0.0.9/cli/broker/export.py
+-rw-r--r--   0        0        0     4133 2024-03-12 09:33:52.748065 remotivelabs_cli-0.0.9/cli/broker/files.py
+-rw-r--r--   0        0        0      141 2024-02-26 09:32:34.931326 remotivelabs_cli-0.0.9/cli/broker/lib/__about__.py
+-rw-r--r--   0        0        0    19713 2024-03-12 09:33:52.748517 remotivelabs_cli-0.0.9/cli/broker/lib/broker.py
+-rw-r--r--   0        0        0     4846 2024-03-12 09:33:52.748919 remotivelabs_cli-0.0.9/cli/broker/playback.py
+-rw-r--r--   0        0        0     1382 2024-03-12 09:33:52.749245 remotivelabs_cli-0.0.9/cli/broker/record.py
+-rw-r--r--   0        0        0     2897 2024-03-12 09:33:52.749553 remotivelabs_cli-0.0.9/cli/broker/scripting.py
+-rw-r--r--   0        0        0     6792 2024-03-12 09:33:52.749955 remotivelabs_cli-0.0.9/cli/broker/signals.py
+-rw-r--r--   0        0        0        1 2023-07-25 06:18:17.910408 remotivelabs_cli-0.0.9/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     3470 2024-02-28 12:15:04.139940 remotivelabs_cli-0.0.9/cli/cloud/auth.py
+-rw-r--r--   0        0        0     3408 2024-02-28 09:16:52.367267 remotivelabs_cli-0.0.9/cli/cloud/auth_tokens.py
+-rw-r--r--   0        0        0     4127 2024-02-28 09:16:52.367702 remotivelabs_cli-0.0.9/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1443 2024-02-28 09:16:52.367911 remotivelabs_cli-0.0.9/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3489 2024-02-28 09:16:52.368159 remotivelabs_cli-0.0.9/cli/cloud/configs.py
+-rw-r--r--   0        0        0     1369 2024-02-28 09:16:52.368526 remotivelabs_cli-0.0.9/cli/cloud/projects.py
+-rw-r--r--   0        0        0    19611 2024-03-12 09:33:52.750406 remotivelabs_cli-0.0.9/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     5885 2024-02-28 09:16:52.368931 remotivelabs_cli-0.0.9/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0      639 2024-02-28 09:16:52.369121 remotivelabs_cli-0.0.9/cli/cloud/sample_recordings.py
+-rw-r--r--   0        0        0     2294 2024-02-28 09:16:52.369341 remotivelabs_cli-0.0.9/cli/cloud/service_account_tokens.py
+-rw-r--r--   0        0        0     1606 2024-02-28 09:16:52.369624 remotivelabs_cli-0.0.9/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0        1 2024-02-01 07:14:42.165748 remotivelabs_cli-0.0.9/cli/connect/__init__.py
+-rw-r--r--   0        0        0     3805 2024-03-12 09:33:52.750881 remotivelabs_cli-0.0.9/cli/connect/connect.py
+-rw-r--r--   0        0        0     5768 2024-03-12 09:33:52.751365 remotivelabs_cli-0.0.9/cli/connect/protopie/protopie.py
+-rw-r--r--   0        0        0     1319 2024-03-12 09:33:52.751625 remotivelabs_cli-0.0.9/cli/errors.py
+-rw-r--r--   0        0        0     1645 2024-02-28 09:16:52.370543 remotivelabs_cli-0.0.9/cli/remotive.py
+-rw-r--r--   0        0        0       78 2023-09-06 06:52:38.303129 remotivelabs_cli-0.0.9/cli/requirements.txt
+-rw-r--r--   0        0        0      792 2024-02-26 09:32:34.938003 remotivelabs_cli-0.0.9/cli/settings.py
+-rw-r--r--   0        0        0        1 2023-12-20 19:10:34.752361 remotivelabs_cli-0.0.9/cli/tools/__init__.py
+-rw-r--r--   0        0        0        1 2023-12-20 19:10:34.752447 remotivelabs_cli-0.0.9/cli/tools/can/__init__.py
+-rw-r--r--   0        0        0     2407 2024-03-12 09:22:15.531516 remotivelabs_cli-0.0.9/cli/tools/can/can.py
+-rw-r--r--   0        0        0     6203 2024-03-11 13:21:18.606814 remotivelabs_cli-0.0.9/cli/tools/can/decoders.py
+-rw-r--r--   0        0        0      198 2023-12-20 19:10:34.752839 remotivelabs_cli-0.0.9/cli/tools/tools.py
+-rw-r--r--   0        0        0      637 2024-03-12 09:34:10.393923 remotivelabs_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.9/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.8/LICENSE` & `remotivelabs_cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/broker/brokers.py` & `remotivelabs_cli-0.0.9/cli/broker/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/broker/export.py` & `remotivelabs_cli-0.0.9/cli/broker/export.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import os
 import signal as os_signal
 from typing import List
 
 import grpc
 import typer
 
+from cli.errors import ErrorPrinter
+
 from .lib.broker import Broker
-from .lib.errors import ErrorPrinter
 
 app = typer.Typer(
     rich_markup_mode="rich",
     help="""
 Export subscribed signals to different formats, currently only InfluxDB line protocol
 but more formats will come soon
 """,
@@ -30,24 +31,24 @@
 ):
     """
     Exports subscribed signals to InfluxDB line-protocol, really useful to dump some signals into
     influxdb for offline analysis and insights.
 
     This is a sample for exporting and importing to InfluxDB using remotive-cli and influx-cli
 
-    [bold]Export:[/bold]
+    Export:
     remotive broker export influxdb --url [URL] --output signals.influx --namespace VehicleBus  \\
         --signal Control.SteeringWheel_Position --signal Control.Accelerator_PedalPosition \\
         --signal GpsPosition.GPS_Longitude --signal GpsPosition.GPS_Latitude
 
-    [bold]Output:[/bold]
+    Output:
     Control, SteeringWheel_Position=1.0,Accelerator_PedalPosition=0,Speed=0 1664787032944374000
     GpsPosition, GPS_Longitude=12.982076,GPS_Latitude=55.618748 1664787032948256000
 
-    [bold]Import:[/bold]
+    Import:
     influx write --org myorg -b my-bucket -p ns --format=lp  -f signals.influx
 
 
     """
 
     if output is not None:
         f = open(output, "w")
```

### Comparing `remotivelabs_cli-0.0.8/cli/broker/files.py` & `remotivelabs_cli-0.0.9/cli/broker/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import os
 from typing import List
 
 import grpc
 import typer
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
+from cli.errors import ErrorPrinter
+
 from .lib.broker import Broker
-from .lib.errors import ErrorPrinter
 
 app = typer.Typer(help=help)
 
 
 @app.command()
 def reload_configuration(
     url: str = typer.Option(..., help="Broker URL", envvar="REMOTIVE_BROKER_URL"),
```

### Comparing `remotivelabs_cli-0.0.8/cli/broker/lib/broker.py` & `remotivelabs_cli-0.0.9/cli/broker/lib/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 import remotivelabs.broker.generated.sync.traffic_api_pb2 as traffic_api
 import remotivelabs.broker.sync as br
 import remotivelabs.broker.sync.helper as br_helper
 import typer
 from rich.console import Console
 
 from cli import settings
-
-from .errors import ErrorPrinter
+from cli.errors import ErrorPrinter
 
 err_console = Console(stderr=True)
 
 
 @dataclass
 class SubscribableSignal:
     name: str
```

### Comparing `remotivelabs_cli-0.0.8/cli/broker/lib/errors.py` & `remotivelabs_cli-0.0.9/cli/errors.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/broker/playback.py` & `remotivelabs_cli-0.0.9/cli/broker/playback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from typing import List
 
 import grpc
 import typer
 
+from cli.errors import ErrorPrinter
+
 from .lib.broker import Broker
-from .lib.errors import ErrorPrinter
 
 app = typer.Typer(help=help)
 
 
 @app.command()
 def play(
     recording: List[str] = typer.Option(..., help="Which recording and which namespace to play"),
```

### Comparing `remotivelabs_cli-0.0.8/cli/broker/record.py` & `remotivelabs_cli-0.0.9/cli/broker/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from typing import List
 
 import grpc
 import typer
 
+from cli.errors import ErrorPrinter
+
 from .lib.broker import Broker
-from .lib.errors import ErrorPrinter
 
 app = typer.Typer(help=help)
 
 
 @app.command()
 def start(
     filename: str = typer.Argument(..., help="Path to local file to upload"),
```

### Comparing `remotivelabs_cli-0.0.8/cli/broker/scripting.py` & `remotivelabs_cli-0.0.9/cli/broker/scripting.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from string import Template
 from typing import List
 
 import typer
 from rich import print as rich_print
 
-from .lib.errors import ErrorPrinter
+from cli.errors import ErrorPrinter
 
 app = typer.Typer(
     rich_markup_mode="rich",
     help="""
 [Experimental] - Generate template lua script for input and output signals
 """,
 )
@@ -24,15 +24,15 @@
     print(f"Secret token written to {path}")
 
 
 @app.command("new-script")
 def new_script(
     input_signal: List[str] = typer.Option(..., help="Required input signal names"),
     output_signal: str = typer.Option(..., help="Name of output signal"),
-    save: bool = typer.Option(False, help="Save file to disk - Default stored as {outout_signal}.lua"),
+    save: bool = typer.Option(False, help="Save file to disk - Default stored as __output_signal__.lua"),
 ):
     def to_subscribable_signal(sig: str) -> tuple[str, str]:
         arr = sig.split(":")
         if len(arr) != 2:
             ErrorPrinter.print_hint(f"--signal must have format namespace:signal ({sig})")
             exit(1)
         return arr[0], arr[1]
```

### Comparing `remotivelabs_cli-0.0.8/cli/broker/signals.py` & `remotivelabs_cli-0.0.9/cli/broker/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 import grpc
 import plotext as plt
 import typer
 from rich import print as rich_rprint
 from typing_extensions import Annotated
 
+from cli.errors import ErrorPrinter
+
 from .lib.broker import Broker, SubscribableSignal
-from .lib.errors import ErrorPrinter
 
 app = typer.Typer(help=help)
 
 
 # signal_values:list = list()
 
 
@@ -60,14 +61,15 @@
     api_key: str = typer.Option(None, help="Cloud Broker API-KEY or access token", envvar="REMOTIVE_BROKER_API_KEY"),
     signal: List[str] = typer.Option(None, help="Signal names to subscribe to, mandatory when not using script"),
     namespace: List[str] = typer.Option(None, help="Deprecated, use --signal namespace:signal"),
     script: Union[
         Annotated[
             Path,
             typer.Option(
+                ...,
                 exists=True,
                 file_okay=True,
                 dir_okay=False,
                 writable=False,
                 readable=True,
                 resolve_path=True,
                 help="Supply a path to Lua script that to use for signal transformation",
```

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/auth.py` & `remotivelabs_cli-0.0.9/cli/cloud/auth.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/auth_tokens.py` & `remotivelabs_cli-0.0.9/cli/cloud/auth_tokens.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.9/cli/cloud/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.9/cli/cloud/cloud_cli.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/configs.py` & `remotivelabs_cli-0.0.9/cli/cloud/configs.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/projects.py` & `remotivelabs_cli-0.0.9/cli/cloud/projects.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.9/cli/cloud/recordings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 import grpc
 import requests
 import typer
 from rich.progress import track
 from typing_extensions import Annotated
 
+from cli.errors import ErrorPrinter
+
 from ..broker.lib.broker import Broker
-from ..broker.lib.errors import ErrorPrinter
 from . import rest_helper as rest
 
 app = typer.Typer()
 
 
 def uid(p):
     print(p)
@@ -191,14 +192,15 @@
 
 
 @app.command()
 def upload(
     path: Annotated[
         Path,
         typer.Argument(
+            ...,
             exists=True,
             file_okay=True,
             dir_okay=False,
             writable=False,
             readable=True,
             resolve_path=True,
             help="Path to recording file to upload",
```

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/rest_helper.py` & `remotivelabs_cli-0.0.9/cli/cloud/rest_helper.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/sample_recordings.py` & `remotivelabs_cli-0.0.9/cli/cloud/sample_recordings.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/service_account_tokens.py` & `remotivelabs_cli-0.0.9/cli/cloud/service_account_tokens.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/cloud/service_accounts.py` & `remotivelabs_cli-0.0.9/cli/cloud/service_accounts.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/remotive.py` & `remotivelabs_cli-0.0.9/cli/remotive.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/settings.py` & `remotivelabs_cli-0.0.9/cli/settings.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/cli/tools/can/can.py` & `remotivelabs_cli-0.0.9/cli/tools/can/can.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.8/pyproject.toml` & `remotivelabs_cli-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remotivelabs-cli"
-version = "0.0.8"
+version = "0.0.9"
 description = "CLI for operating RemotiveCloud and RemotiveBroker"
 authors = ["Johan Rask <johan.rask@remotivelabs.com>"]
 readme = "README.md"
 packages = [{include = "cli"}]
 
 [tool.poetry.dependencies]
 trogon = ">=0.5.0"
```

### Comparing `remotivelabs_cli-0.0.8/PKG-INFO` & `remotivelabs_cli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI for operating RemotiveCloud and RemotiveBroker
 Author: Johan Rask
 Author-email: johan.rask@remotivelabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

