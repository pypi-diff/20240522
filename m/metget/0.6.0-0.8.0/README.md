# Comparing `tmp/metget-0.6.0.tar.gz` & `tmp/metget-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metget-0.6.0.tar", last modified: Tue Mar  5 00:08:43 2024, max compression
+gzip compressed data, was "metget-0.8.0.tar", last modified: Wed May 22 00:39:54 2024, max compression
```

## Comparing `metget-0.6.0.tar` & `metget-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-03-05 00:08:43.625698 metget-0.6.0/
--rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.6.0/LICENSE.md
--rw-r--r--   0 zcobell    (502) staff       (20)    11994 2024-03-05 00:08:43.625438 metget-0.6.0/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)    11001 2023-12-21 16:31:18.000000 metget-0.6.0/README.md
--rw-r--r--   0 zcobell    (502) staff       (20)     2933 2024-03-05 00:06:36.000000 metget-0.6.0/pyproject.toml
--rw-r--r--   0 zcobell    (502) staff       (20)       38 2024-03-05 00:08:43.625748 metget-0.6.0/setup.cfg
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-03-05 00:08:43.618651 metget-0.6.0/src/
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-03-05 00:08:43.622189 metget-0.6.0/src/metget/
--rw-r--r--   0 zcobell    (502) staff       (20)       68 2024-03-05 00:06:36.000000 metget-0.6.0/src/metget/__init__.py
--rw-r--r--   0 zcobell    (502) staff       (20)    20142 2024-03-05 00:05:19.000000 metget-0.6.0/src/metget/metget_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)    10348 2023-12-20 17:17:29.000000 metget-0.6.0/src/metget/metget_client.py
--rw-r--r--   0 zcobell    (502) staff       (20)     3073 2023-12-20 17:03:48.000000 metget-0.6.0/src/metget/metget_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2913 2024-03-05 00:05:19.000000 metget-0.6.0/src/metget/metget_data.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2819 2023-12-20 17:18:16.000000 metget-0.6.0/src/metget/metget_environment.py
--rw-r--r--   0 zcobell    (502) staff       (20)    20916 2024-03-05 00:05:19.000000 metget-0.6.0/src/metget/metget_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     4027 2023-12-20 15:21:14.000000 metget-0.6.0/src/metget/metget_track.py
--rw-r--r--   0 zcobell    (502) staff       (20)     5771 2023-12-20 15:21:14.000000 metget-0.6.0/src/metget/spinnerlogger.py
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-03-05 00:08:43.625168 metget-0.6.0/src/metget.egg-info/
--rw-r--r--   0 zcobell    (502) staff       (20)    11994 2024-03-05 00:08:43.000000 metget-0.6.0/src/metget.egg-info/PKG-INFO
--rw-r--r--   0 zcobell    (502) staff       (20)      586 2024-03-05 00:08:43.000000 metget-0.6.0/src/metget.egg-info/SOURCES.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        1 2024-03-05 00:08:43.000000 metget-0.6.0/src/metget.egg-info/dependency_links.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       52 2024-03-05 00:08:43.000000 metget-0.6.0/src/metget.egg-info/entry_points.txt
--rw-r--r--   0 zcobell    (502) staff       (20)       26 2024-03-05 00:08:43.000000 metget-0.6.0/src/metget.egg-info/requires.txt
--rw-r--r--   0 zcobell    (502) staff       (20)        7 2024-03-05 00:08:43.000000 metget-0.6.0/src/metget.egg-info/top_level.txt
-drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-03-05 00:08:43.624772 metget-0.6.0/test/
--rw-r--r--   0 zcobell    (502) staff       (20)    26116 2024-03-05 00:05:19.000000 metget-0.6.0/test/test_build.py
--rw-r--r--   0 zcobell    (502) staff       (20)      233 2023-11-21 21:19:02.000000 metget-0.6.0/test/test_cli.py
--rw-r--r--   0 zcobell    (502) staff       (20)     1722 2023-12-20 17:07:19.000000 metget-0.6.0/test/test_credits.py
--rw-r--r--   0 zcobell    (502) staff       (20)    10500 2024-03-05 00:05:19.000000 metget-0.6.0/test/test_status.py
--rw-r--r--   0 zcobell    (502) staff       (20)     2599 2023-12-20 15:25:51.000000 metget-0.6.0/test/test_track.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-05-22 00:39:54.136822 metget-0.8.0/
+-rw-r--r--   0 zcobell    (502) staff       (20)     1115 2023-07-08 15:49:08.000000 metget-0.8.0/LICENSE.md
+-rw-r--r--   0 zcobell    (502) staff       (20)    11994 2024-05-22 00:39:54.136586 metget-0.8.0/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)    11001 2023-12-21 16:31:18.000000 metget-0.8.0/README.md
+-rw-r--r--   0 zcobell    (502) staff       (20)     2933 2024-05-22 00:38:21.000000 metget-0.8.0/pyproject.toml
+-rw-r--r--   0 zcobell    (502) staff       (20)       38 2024-05-22 00:39:54.136865 metget-0.8.0/setup.cfg
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-05-22 00:39:54.129247 metget-0.8.0/src/
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-05-22 00:39:54.133369 metget-0.8.0/src/metget/
+-rw-r--r--   0 zcobell    (502) staff       (20)       68 2024-05-22 00:38:21.000000 metget-0.8.0/src/metget/__init__.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    20263 2024-05-22 00:37:56.000000 metget-0.8.0/src/metget/metget_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    10462 2024-05-22 00:37:56.000000 metget-0.8.0/src/metget/metget_client.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     3073 2023-12-20 17:03:48.000000 metget-0.8.0/src/metget/metget_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2909 2024-05-22 00:37:56.000000 metget-0.8.0/src/metget/metget_data.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2819 2023-12-20 17:18:16.000000 metget-0.8.0/src/metget/metget_environment.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    21325 2024-05-22 00:37:56.000000 metget-0.8.0/src/metget/metget_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     4027 2023-12-20 15:21:14.000000 metget-0.8.0/src/metget/metget_track.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     5790 2024-05-22 00:37:56.000000 metget-0.8.0/src/metget/spinnerlogger.py
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-05-22 00:39:54.136264 metget-0.8.0/src/metget.egg-info/
+-rw-r--r--   0 zcobell    (502) staff       (20)    11994 2024-05-22 00:39:54.000000 metget-0.8.0/src/metget.egg-info/PKG-INFO
+-rw-r--r--   0 zcobell    (502) staff       (20)      586 2024-05-22 00:39:54.000000 metget-0.8.0/src/metget.egg-info/SOURCES.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        1 2024-05-22 00:39:54.000000 metget-0.8.0/src/metget.egg-info/dependency_links.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       52 2024-05-22 00:39:54.000000 metget-0.8.0/src/metget.egg-info/entry_points.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)       26 2024-05-22 00:39:54.000000 metget-0.8.0/src/metget.egg-info/requires.txt
+-rw-r--r--   0 zcobell    (502) staff       (20)        7 2024-05-22 00:39:54.000000 metget-0.8.0/src/metget.egg-info/top_level.txt
+drwxr-xr-x   0 zcobell    (502) staff       (20)        0 2024-05-22 00:39:54.135980 metget-0.8.0/test/
+-rw-r--r--   0 zcobell    (502) staff       (20)    26116 2024-03-05 00:05:19.000000 metget-0.8.0/test/test_build.py
+-rw-r--r--   0 zcobell    (502) staff       (20)      233 2023-11-21 21:19:02.000000 metget-0.8.0/test/test_cli.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     1722 2023-12-20 17:07:19.000000 metget-0.8.0/test/test_credits.py
+-rw-r--r--   0 zcobell    (502) staff       (20)    10578 2024-05-22 00:37:56.000000 metget-0.8.0/test/test_status.py
+-rw-r--r--   0 zcobell    (502) staff       (20)     2599 2023-12-20 15:25:51.000000 metget-0.8.0/test/test_track.py
```

### Comparing `metget-0.6.0/LICENSE.md` & `metget-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/PKG-INFO` & `metget-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.6.0
+Version: 0.8.0
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.6.0/README.md` & `metget-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/pyproject.toml` & `metget-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metget"
-version = "0.6.0"
+version = "0.8.0"
 description = "A client package for interaction with a MetGet server instance"
 authors = [
     { name = "Zach Cobell", email = "zcobell@thewaterinstitute.org" },
 ]
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.8"
@@ -40,15 +40,15 @@
 [tool.setuptools.dynamic]
 version = { attr = "metget.__version__" }
 
 [project.scripts]
 metget = "metget:metget_client_cli"
 
 [tool.bumpver]
-current_version = "0.6.0"
+current_version = "0.8.0"
 version_pattern = 'MAJOR.MINOR.PATCH[PYTAGNUM]'
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `metget-0.6.0/src/metget/metget_build.py` & `metget-0.8.0/src/metget/metget_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #
 ###################################################################################################
 
 import argparse
 import contextlib
 import json
 import time
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import Tuple, Union
 
 from .metget_data import AVAILABLE_MODELS
 
 
 class MetGetBuildRest:
     def __init__(
@@ -102,15 +102,15 @@
                 year = int(keys[1])
                 basin = keys[2]
                 storm = keys[3]
                 advisory = keys[4]
                 with contextlib.suppress(ValueError):
                     advisory = f"{int(advisory):03d}"
             else:
-                year = datetime.utcnow().year
+                year = datetime.now(timezone.utc).year
                 basin = keys[1]
                 storm = keys[2]
                 advisory = keys[3]
                 with contextlib.suppress(ValueError):
                     advisory = f"{int(advisory):03d}"
             model = "nhc"
         else:
@@ -327,39 +327,39 @@
             max_wait (int): Maximum time to wait for data to appear
             output_directory (Union[str, None]): Output directory
 
         Returns:
             None
         """
         import os
-        from datetime import datetime, timedelta
+        from datetime import datetime, timedelta, timezone
 
         import requests
 
         from .spinnerlogger import SpinnerLogger
 
         # ...Wait time
-        end_time = datetime.utcnow() + timedelta(hours=max_wait)
+        end_time = datetime.now(timezone.utc) + timedelta(hours=max_wait)
 
         # ...Timing information
-        request_start_time = datetime.utcnow()
+        request_start_time = datetime.now(timezone.utc)
 
         # ...Wait for request data to appear
         tries = 0
         data_ready = False
         status = None
 
         spinner = SpinnerLogger()
         print(f"Waiting for request id {data_id:s}", flush=True)
         spinner.start()
 
         return_data = None
         data_url = None
 
-        while datetime.utcnow() <= end_time:
+        while datetime.now(timezone.utc) <= end_time:
             tries += 1
             try:
                 data_url, status = self.check_metget_status(data_id)
                 spinner.set_text(SpinnerLogger.standard_log(tries, status))
                 if status == "completed":
                     spinner.succeed()
                     # ...Parse the return to get data
@@ -391,29 +391,31 @@
                     if not os.path.exists(output_directory):
                         msg = f"Output directory does not exist: {output_directory:s}"
                         raise RuntimeError(msg)
                     ff = os.path.join(output_directory, f)
                 else:
                     ff = f
 
-                time_stamp = datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S UTC")
+                time_stamp = datetime.now(timezone.utc).strftime(
+                    "%Y-%m-%d %H:%M:%S UTC"
+                )
                 spinner.start(f"[{time_stamp:s}]: Getting file: {f:s}")
                 with requests.get(data_url + "/" + f, stream=True) as r:
                     r.raise_for_status()
                     with open(ff, "wb") as wind_file:
                         for chunk in r.iter_content(chunk_size=8192):
                             wind_file.write(chunk)
                 spinner.succeed()
 
-            request_end_time = datetime.utcnow()
+            request_end_time = datetime.now(timezone.utc)
             request_duration = request_end_time - request_start_time
             hours, remainder = divmod(request_duration.total_seconds(), 3600)
             minutes, seconds = divmod(remainder, 60)
 
-            time_stamp = datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S UTC")
+            time_stamp = datetime.now(timezone.utc).strftime("%Y-%m-%d %H:%M:%S UTC")
             spinner.succeed(
                 "[{:s}]: Elapsed time: {:d}h{:02d}m{:02d}s".format(
                     time_stamp, int(hours), int(minutes), int(seconds)
                 )
             )
         else:
             if status == "restore":
```

### Comparing `metget-0.6.0/src/metget/metget_client.py` & `metget-0.8.0/src/metget/metget_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,17 @@
         help="Ensemble member to request data for",
         type=str,
         metavar="s",
     )
     status.add_argument(
         "--format", help="Output format (json, pretty)", metavar="f", default="pretty"
     )
+    status.add_argument(
+        "--complete", help="Only show data which is complete", action="store_true"
+    )
 
 
 def initialize_track_cli(subparsers) -> None:
     """
     This method is used to initialize the track subparser
 
     Returns:
```

### Comparing `metget-0.6.0/src/metget/metget_credits.py` & `metget-0.8.0/src/metget/metget_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/src/metget/metget_data.py` & `metget-0.8.0/src/metget/metget_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 # Available metget models
 AVAILABLE_MODELS = {
     "gfs": "gfs-ncep",
     "gefs": "gefs-ncep",
     "nam": "nam-ncep",
     "hwrf": "hwrf",
-    "hrrr": "hrrr-ncep",
-    "hrrr-alaska": "hrrr-alaska-ncep",
+    "hrrr": "hrrr-conus",
+    "hrrr-alaska": "hrrr-alaska",
     "hafsa": "ncep-hafs-a",
     "hafsb": "ncep-hafs-b",
     "wpc": "wpc-ncep",
     "coamps": "coamps-tc",
     "ctcx": "coamps-ctcx",
     "nhc": "nhc",
     "era5": "era5",
```

### Comparing `metget-0.6.0/src/metget/metget_environment.py` & `metget-0.8.0/src/metget/metget_environment.py`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/src/metget/metget_status.py` & `metget-0.8.0/src/metget/metget_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,22 @@
 
         Args:
             url: The url to add the start and end parameters to
 
         Returns:
             The url with the start and end parameters added
         """
-        from datetime import datetime
+        from datetime import datetime, timezone
 
         if self.__args.start:
             url += "&start={:s}".format(self.__args.start.strftime("%Y-%m-%d"))
             if not self.__args.end:
-                url += "&end={:s}".format(datetime.utcnow().strftime("%Y-%m-%d"))
+                url += "&end={:s}".format(
+                    datetime.now(timezone.utc).strftime("%Y-%m-%d")
+                )
             else:
                 url += "&end={:s}".format(self.__args.end.strftime("%Y-%m-%d"))
         return url
 
     # TODO: ERA5 Hindcast
     # def __status_hindcast(self, model: str) -> None:
     #     import json
@@ -265,15 +267,17 @@
             print(json.dumps(data))
         elif self.__args.format == "pretty":
             if self.__args.storm and self.__args.ensemble_member:
                 model_name = "{:s}-{:s}-{:s}".format(
                     model, self.__args.storm, self.__args.ensemble_member
                 )
                 self.__print_status_generic(
-                    model_name, data[self.__args.storm][self.__args.ensemble_member]
+                    model_name,
+                    data[self.__args.storm][self.__args.ensemble_member],
+                    self.__args.complete,
                 )
             else:
                 table = prettytable.PrettyTable(
                     [
                         "Storm",
                         "First Forecast Cycle",
                         "Last Forecast Cycle",
@@ -341,15 +345,17 @@
         response = requests.get(
             url, headers={"x-api-key": self.__environment["apikey"]}
         )
 
         if self.__args.ensemble_member:
             model_name = f"{model:s}-{self.__args.ensemble_member:s}"
             self.__print_status_generic(
-                model_name, response.json()["body"][self.__args.ensemble_member]
+                model_name,
+                response.json()["body"][self.__args.ensemble_member],
+                self.__args.complete,
             )
         else:
             self.__print_status_multi("ensemble", model, response.json()["body"])
 
     def __status_synoptic(self, model: str) -> None:
         """
         This method is used to get the status of the synoptic data
@@ -366,15 +372,17 @@
         url = self.__add_url_start_end_parameters(url)
 
         # ...Get the json from the endpoint
         response = requests.get(
             url, headers={"x-api-key": self.__environment["apikey"]}
         )
 
-        self.__print_status_generic(model.upper(), response.json()["body"])
+        self.__print_status_generic(
+            model.upper(), response.json()["body"], self.__args.complete
+        )
 
     def __status_synoptic_storm(self, model: str) -> None:
         """
         This method is used to get the status of the synoptic data for storms
 
         Args:
             model: The model to get the status for
@@ -434,15 +442,17 @@
                     if "year" not in self.__args:
                         print("[ERROR]: Must provide a year")
                         exit(1)
                     else:
                         year = self.__args.year
                 else:
                     year = next(iter(data.keys()))
-                self.__print_status_generic(model_name, data[year][self.__args.storm])
+                self.__print_status_generic(
+                    model_name, data[year][self.__args.storm], self.__args.complete
+                )
             else:
                 if data_type == "ensemble":
                     table = prettytable.PrettyTable(
                         [
                             "Ensemble Member",
                             "First Forecast Cycle",
                             "Last Forecast Cycle",
@@ -501,15 +511,17 @@
                     print(
                         "Status for {:s} Model Storms (class: {:s})".format(
                             model.upper(), self.__model_class
                         )
                     )
                     print(table.get_string(sortby="First Forecast Cycle"))
 
-    def __print_status_generic(self, model: str, data: dict) -> None:
+    def __print_status_generic(
+        self, model: str, data: dict, only_complete: bool
+    ) -> None:
         """
         This method is used to get the status of a generic format
 
         Args:
             model: The model to get the status for
             data: The data to get the status for
 
@@ -530,22 +542,24 @@
             table = prettytable.PrettyTable(["Forecast Cycle", "End Time", "Status"])
 
             for cycle in data["cycles"]:
                 if cycle["cycle"] in complete_cycles:
                     status = "complete"
                 else:
                     status = "incomplete ({:d})".format(cycle["duration"])
-                table.add_row(
-                    [
-                        cycle["cycle"],
-                        datetime.strptime(cycle["cycle"], "%Y-%m-%d %H:%M:%S")
-                        + timedelta(hours=cycle["duration"]),
-                        status,
-                    ]
-                )
+
+                if status == "complete" or not only_complete:
+                    table.add_row(
+                        [
+                            cycle["cycle"],
+                            datetime.strptime(cycle["cycle"], "%Y-%m-%d %H:%M:%S")
+                            + timedelta(hours=cycle["duration"]),
+                            status,
+                        ]
+                    )
 
             print(table)
 
 
 def metget_status(args: argparse.Namespace) -> None:
     """
     This method is used to get the status of the metget data
```

### Comparing `metget-0.6.0/src/metget/metget_track.py` & `metget-0.8.0/src/metget/metget_track.py`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/src/metget/spinnerlogger.py` & `metget-0.8.0/src/metget/spinnerlogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     def __time_str() -> str:
         """
         Returns the current time in UTC
 
         Returns:
             str: Current time in UTC
         """
-        from datetime import datetime
+        from datetime import datetime, timezone
 
-        return datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S UTC")
+        return datetime.now(timezone.utc).strftime("%Y-%m-%d %H:%M:%S UTC")
 
     def start(self, text: Optional[str] = None) -> None:
         """
         Starts the spinner animation
 
         Args:
             text (str, optional): Text to display. Defaults to None.
```

### Comparing `metget-0.6.0/src/metget.egg-info/PKG-INFO` & `metget-0.8.0/src/metget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metget
-Version: 0.6.0
+Version: 0.8.0
 Summary: A client package for interaction with a MetGet server instance
 Author-email: Zach Cobell <zcobell@thewaterinstitute.org>
 License: MIT
 Project-URL: Homepage, https://github.com/waterinstitute/metget
 Project-URL: Bug Reports, https://github.com/waterinstitute/metget/issues
 Project-URL: Source, https://github.com/waterinstitute/metget
 Keywords: forecast,meteorology,stormsurge
```

### Comparing `metget-0.6.0/src/metget.egg-info/SOURCES.txt` & `metget-0.8.0/src/metget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/test/test_build.py` & `metget-0.8.0/test/test_build.py`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/test/test_credits.py` & `metget-0.8.0/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `metget-0.6.0/test/test_status.py` & `metget-0.8.0/test/test_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     import json
 
     args = argparse.Namespace()
     args.model = "gfs"
     args.format = "pretty"
     args.start = None
     args.end = None
+    args.complete = False
     args.endpoint = METGET_DMY_ENDPOINT
     args.apikey = METGET_DMY_APIKEY
     args.api_version = METGET_API_VERSION
 
     s = MetGetStatus(args)
     with requests_mock.Mocker() as m:
         m.get(METGET_DMY_ENDPOINT + "/status?model=gfs", json=GFS_STATUS_JSON)
@@ -83,14 +84,15 @@
     from datetime import datetime
 
     args = argparse.Namespace()
     args.model = "hwrf"
     args.format = "pretty"
     args.start = datetime(2023, 6, 1)
     args.storm = None
+    args.complete = False
     args.end = datetime(2023, 7, 11)
     args.endpoint = METGET_DMY_ENDPOINT
     args.apikey = METGET_DMY_APIKEY
     args.api_version = METGET_API_VERSION
 
     s = MetGetStatus(args)
     url = (
@@ -216,14 +218,15 @@
     args = argparse.Namespace()
     args.model = "gefs"
     args.start = datetime(2023, 6, 1)
     args.end = datetime(2023, 6, 8)
     args.ensemble_member = "c00"
     args.format = "json"
     args.storm = None
+    args.complete = False
     args.endpoint = METGET_DMY_ENDPOINT
     args.apikey = METGET_DMY_APIKEY
     args.api_version = METGET_API_VERSION
 
     with requests_mock.Mocker() as m:
         m.get(
             METGET_DMY_ENDPOINT
```

### Comparing `metget-0.6.0/test/test_track.py` & `metget-0.8.0/test/test_track.py`

 * *Files identical despite different names*

