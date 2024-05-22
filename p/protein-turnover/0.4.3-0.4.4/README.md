# Comparing `tmp/protein_turnover-0.4.3.tar.gz` & `tmp/protein_turnover-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_turnover-0.4.3.tar", max compression
+gzip compressed data, was "protein_turnover-0.4.4.tar", max compression
```

## Comparing `protein_turnover-0.4.3.tar` & `protein_turnover-0.4.4.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.4.3/LICENSE
--rw-r--r--   0        0        0       54 2024-05-20 06:25:28.823906 protein_turnover-0.4.3/prerelease.md
--rw-r--r--   0        0        0    16384 2024-05-22 01:44:28.646339 protein_turnover-0.4.3/protein_turnover/.web.py.swp
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.4.3/protein_turnover/__init__.py
--rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.4.3/protein_turnover/__main__.py
--rw-r--r--   0        0        0      140 2024-05-20 06:14:30.276214 protein_turnover-0.4.3/protein_turnover/api.py
--rw-r--r--   0        0        0    11218 2024-05-17 13:48:47.050662 protein_turnover-0.4.3/protein_turnover/background.py
--rw-r--r--   0        0        0     1619 2024-05-19 20:50:27.558491 protein_turnover-0.4.3/protein_turnover/background_ui.py
--rw-r--r--   0        0        0     6670 2024-05-18 20:24:19.465998 protein_turnover-0.4.3/protein_turnover/broken_api.py
--rw-r--r--   0        0        0     2706 2024-05-19 21:11:19.897073 protein_turnover-0.4.3/protein_turnover/cli.py
--rw-r--r--   0        0        0     1120 2024-05-20 01:32:55.419976 protein_turnover-0.4.3/protein_turnover/config.py
--rw-r--r--   0        0        0     2430 2024-05-20 01:32:50.255985 protein_turnover-0.4.3/protein_turnover/config2.py
--rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.4.3/protein_turnover/dinosaur/__init__.py
--rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.4.3/protein_turnover/dinosaur/cmd.py
--rw-r--r--   0        0        0     1914 2024-05-19 04:54:45.120734 protein_turnover-0.4.3/protein_turnover/dinosaur/dinosaur.py
--rw-r--r--   0        0        0      393 2024-05-18 20:23:03.965361 protein_turnover-0.4.3/protein_turnover/exts.py
--rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.4.3/protein_turnover/filters.py
--rw-r--r--   0        0        0    19857 2024-05-19 21:41:27.580566 protein_turnover-0.4.3/protein_turnover/fitenvelopes.py
--rw-r--r--   0        0        0     8516 2024-05-17 11:31:30.621734 protein_turnover-0.4.3/protein_turnover/jobs.py
--rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.4.3/protein_turnover/logger.py
--rw-r--r--   0        0        0      979 2024-05-20 01:33:43.899913 protein_turnover-0.4.3/protein_turnover/mailer.py
--rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.4.3/protein_turnover/parallel_utils.py
--rw-r--r--   0        0        0    12689 2024-05-17 05:04:12.311778 protein_turnover-0.4.3/protein_turnover/pepxml.py
--rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.4.3/protein_turnover/pepxml_reader.py
--rw-r--r--   0        0        0    17519 2024-05-20 01:31:09.608194 protein_turnover-0.4.3/protein_turnover/plotting.py
--rw-r--r--   0        0        0     3826 2024-05-17 05:04:43.620071 protein_turnover-0.4.3/protein_turnover/protxml.py
--rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.4.3/protein_turnover/py.typed
--rw-r--r--   0        0        0    27984 2024-05-20 06:17:31.161204 protein_turnover-0.4.3/protein_turnover/pymz.py
--rw-r--r--   0        0        0    11026 2024-05-19 21:11:20.217076 protein_turnover-0.4.3/protein_turnover/pymz_ui.py
--rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.4.3/protein_turnover/settings.py
--rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.4.3/protein_turnover/sns.py
--rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.4.3/protein_turnover/sqla/__init__.py
--rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.4.3/protein_turnover/sqla/iso_peaks.py
--rw-r--r--   0        0        0     4009 2024-05-19 21:11:19.197067 protein_turnover-0.4.3/protein_turnover/sqla/iso_peaks_ui.py
--rw-r--r--   0        0        0    12901 2024-05-17 05:11:50.442492 protein_turnover-0.4.3/protein_turnover/sqla/model.py
--rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.4.3/protein_turnover/sqla/query.py
--rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.4.3/protein_turnover/sqla/utils.py
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.4.3/protein_turnover/types/__init__.py
--rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.4.3/protein_turnover/types/checking.py
--rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.4.3/protein_turnover/types/mzmltypes.py
--rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.4.3/protein_turnover/types/pepxmltypes.py
--rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.4.3/protein_turnover/types/turnovertype.py
--rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.4.3/protein_turnover/unimod.py
--rw-r--r--   0        0        0    21118 2024-05-18 20:30:54.981335 protein_turnover-0.4.3/protein_turnover/utils.py
--rw-r--r--   0        0        0    10302 2024-05-22 03:03:26.632244 protein_turnover-0.4.3/protein_turnover/web.py
--rw-r--r--   0        0        0     6393 2024-05-19 21:26:54.413011 protein_turnover-0.4.3/protein_turnover/web_ui.py
--rw-r--r--   0        0        0     1484 2024-05-22 03:03:39.920347 protein_turnover-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 protein_turnover-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.4.4/LICENSE
+-rw-r--r--   0        0        0       54 2024-05-20 06:25:28.823906 protein_turnover-0.4.4/prerelease.md
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.4.4/protein_turnover/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.4.4/protein_turnover/__main__.py
+-rw-r--r--   0        0        0      140 2024-05-20 06:14:30.276214 protein_turnover-0.4.4/protein_turnover/api.py
+-rw-r--r--   0        0        0    11218 2024-05-17 13:48:47.050662 protein_turnover-0.4.4/protein_turnover/background.py
+-rw-r--r--   0        0        0     1619 2024-05-19 20:50:27.558491 protein_turnover-0.4.4/protein_turnover/background_ui.py
+-rw-r--r--   0        0        0     6670 2024-05-18 20:24:19.465998 protein_turnover-0.4.4/protein_turnover/broken_api.py
+-rw-r--r--   0        0        0     2706 2024-05-19 21:11:19.897073 protein_turnover-0.4.4/protein_turnover/cli.py
+-rw-r--r--   0        0        0     1120 2024-05-20 01:32:55.419976 protein_turnover-0.4.4/protein_turnover/config.py
+-rw-r--r--   0        0        0     2430 2024-05-20 01:32:50.255985 protein_turnover-0.4.4/protein_turnover/config2.py
+-rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.4.4/protein_turnover/dinosaur/__init__.py
+-rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.4.4/protein_turnover/dinosaur/cmd.py
+-rw-r--r--   0        0        0     1914 2024-05-19 04:54:45.120734 protein_turnover-0.4.4/protein_turnover/dinosaur/dinosaur.py
+-rw-r--r--   0        0        0      393 2024-05-18 20:23:03.965361 protein_turnover-0.4.4/protein_turnover/exts.py
+-rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.4.4/protein_turnover/filters.py
+-rw-r--r--   0        0        0    19857 2024-05-19 21:41:27.580566 protein_turnover-0.4.4/protein_turnover/fitenvelopes.py
+-rw-r--r--   0        0        0     8516 2024-05-17 11:31:30.621734 protein_turnover-0.4.4/protein_turnover/jobs.py
+-rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.4.4/protein_turnover/logger.py
+-rw-r--r--   0        0        0      979 2024-05-20 01:33:43.899913 protein_turnover-0.4.4/protein_turnover/mailer.py
+-rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.4.4/protein_turnover/parallel_utils.py
+-rw-r--r--   0        0        0    12689 2024-05-17 05:04:12.311778 protein_turnover-0.4.4/protein_turnover/pepxml.py
+-rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.4.4/protein_turnover/pepxml_reader.py
+-rw-r--r--   0        0        0    17519 2024-05-20 01:31:09.608194 protein_turnover-0.4.4/protein_turnover/plotting.py
+-rw-r--r--   0        0        0     3826 2024-05-17 05:04:43.620071 protein_turnover-0.4.4/protein_turnover/protxml.py
+-rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.4.4/protein_turnover/py.typed
+-rw-r--r--   0        0        0    27984 2024-05-20 06:17:31.161204 protein_turnover-0.4.4/protein_turnover/pymz.py
+-rw-r--r--   0        0        0    11026 2024-05-19 21:11:20.217076 protein_turnover-0.4.4/protein_turnover/pymz_ui.py
+-rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.4.4/protein_turnover/settings.py
+-rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.4.4/protein_turnover/sns.py
+-rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.4.4/protein_turnover/sqla/__init__.py
+-rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.4.4/protein_turnover/sqla/iso_peaks.py
+-rw-r--r--   0        0        0     4009 2024-05-19 21:11:19.197067 protein_turnover-0.4.4/protein_turnover/sqla/iso_peaks_ui.py
+-rw-r--r--   0        0        0    12901 2024-05-17 05:11:50.442492 protein_turnover-0.4.4/protein_turnover/sqla/model.py
+-rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.4.4/protein_turnover/sqla/query.py
+-rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.4.4/protein_turnover/sqla/utils.py
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.4.4/protein_turnover/types/__init__.py
+-rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.4.4/protein_turnover/types/checking.py
+-rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.4.4/protein_turnover/types/mzmltypes.py
+-rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.4.4/protein_turnover/types/pepxmltypes.py
+-rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.4.4/protein_turnover/types/turnovertype.py
+-rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.4.4/protein_turnover/unimod.py
+-rw-r--r--   0        0        0    21118 2024-05-18 20:30:54.981335 protein_turnover-0.4.4/protein_turnover/utils.py
+-rw-r--r--   0        0        0    10318 2024-05-22 03:17:24.410815 protein_turnover-0.4.4/protein_turnover/web.py
+-rw-r--r--   0        0        0     6393 2024-05-19 21:26:54.413011 protein_turnover-0.4.4/protein_turnover/web_ui.py
+-rw-r--r--   0        0        0     1484 2024-05-22 03:15:20.181836 protein_turnover-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 protein_turnover-0.4.4/PKG-INFO
```

### Comparing `protein_turnover-0.4.3/LICENSE` & `protein_turnover-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/background.py` & `protein_turnover-0.4.4/protein_turnover/background.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/background_ui.py` & `protein_turnover-0.4.4/protein_turnover/background_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/broken_api.py` & `protein_turnover-0.4.4/protein_turnover/broken_api.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/cli.py` & `protein_turnover-0.4.4/protein_turnover/cli.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/config.py` & `protein_turnover-0.4.4/protein_turnover/config.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/config2.py` & `protein_turnover-0.4.4/protein_turnover/config2.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/dinosaur/cmd.py` & `protein_turnover-0.4.4/protein_turnover/dinosaur/cmd.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/dinosaur/dinosaur.py` & `protein_turnover-0.4.4/protein_turnover/dinosaur/dinosaur.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/filters.py` & `protein_turnover-0.4.4/protein_turnover/filters.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/fitenvelopes.py` & `protein_turnover-0.4.4/protein_turnover/fitenvelopes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/jobs.py` & `protein_turnover-0.4.4/protein_turnover/jobs.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/logger.py` & `protein_turnover-0.4.4/protein_turnover/logger.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/mailer.py` & `protein_turnover-0.4.4/protein_turnover/mailer.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/parallel_utils.py` & `protein_turnover-0.4.4/protein_turnover/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/pepxml.py` & `protein_turnover-0.4.4/protein_turnover/pepxml.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/pepxml_reader.py` & `protein_turnover-0.4.4/protein_turnover/pepxml_reader.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/plotting.py` & `protein_turnover-0.4.4/protein_turnover/plotting.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/protxml.py` & `protein_turnover-0.4.4/protein_turnover/protxml.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/pymz.py` & `protein_turnover-0.4.4/protein_turnover/pymz.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/pymz_ui.py` & `protein_turnover-0.4.4/protein_turnover/pymz_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/settings.py` & `protein_turnover-0.4.4/protein_turnover/settings.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/sns.py` & `protein_turnover-0.4.4/protein_turnover/sns.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/sqla/iso_peaks.py` & `protein_turnover-0.4.4/protein_turnover/sqla/iso_peaks.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/sqla/iso_peaks_ui.py` & `protein_turnover-0.4.4/protein_turnover/sqla/iso_peaks_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/sqla/model.py` & `protein_turnover-0.4.4/protein_turnover/sqla/model.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/sqla/query.py` & `protein_turnover-0.4.4/protein_turnover/sqla/query.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/sqla/utils.py` & `protein_turnover-0.4.4/protein_turnover/sqla/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/types/checking.py` & `protein_turnover-0.4.4/protein_turnover/types/checking.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/types/mzmltypes.py` & `protein_turnover-0.4.4/protein_turnover/types/mzmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/types/pepxmltypes.py` & `protein_turnover-0.4.4/protein_turnover/types/pepxmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/types/turnovertype.py` & `protein_turnover-0.4.4/protein_turnover/types/turnovertype.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/unimod.py` & `protein_turnover-0.4.4/protein_turnover/unimod.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/utils.py` & `protein_turnover-0.4.4/protein_turnover/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/protein_turnover/web.py` & `protein_turnover-0.4.4/protein_turnover/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import signal
 import subprocess
 import sys
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from tempfile import NamedTemporaryFile
+from tempfile import TemporaryDirectory
 from threading import Thread
 from types import ModuleType
 from typing import Any
 from typing import Callable
 from typing import TypedDict
 
 import click
@@ -64,26 +64,24 @@
 
         kwargs = PopenArgs(creationflags=0, preexec_fn=None)
         if self.prevent_sig:
             if sys.platform == "win32":
                 kwargs["creationflags"] = (
                     subprocess.CREATE_NEW_PROCESS_GROUP
                 )
-                shell = True
             else:
-                shell = self.shell
                 if sys.version_info >= (3, 11):
                     kwargs["process_group"] = 0
                 else:
                     kwargs["preexec_fn"] = os.setpgrp
         return subprocess.Popen(  # type: ignore
             self.cmd,
             cwd=self.directory,
             env=self.getenv(),
-            shell=shell,
+            shell=self.shell,
             **kwargs,
         )
 
 
 def browser(url: str = "http://127.0.0.1:8000", sleep: float = 5.0) -> Thread:
     import webbrowser
 
@@ -249,46 +247,48 @@
             ],
             directory=".",
             prevent_sig=True,
         )
     Url = f"127.0.0.1:{port}"
     if page is not None:
         Url += f"/{page}"
-    with NamedTemporaryFile("w+b") as fp:
-        tomli_w.dump(web_conf, fp)  # type: ignore
-        fp.flush()
+    with TemporaryDirectory() as td:
+        filename = Path(td) / 'flask.cfg'
+        with filename.open('wb') as fp:
+            tomli_w.dump(web_conf, fp)  # type: ignore
+
 
         if not gunicorn:
             website = Runner(
                 "flask",
                 [
                     sys.executable,
                     "-m",
                     "flask",
                     "--app",
                     flask_app,
                     "run",
                     f"--port={port}",
                     *server_options,
                 ],
-                env={"TURNOVER_SETTINGS": fp.name, "FLASK_DEBUG": "0"},
+                env={"TURNOVER_SETTINGS": str(filename), "FLASK_DEBUG": "0"},
                 prevent_sig=True,
             )
         else:
             website = Runner(
                 "gunicorn",
                 [
                     sys.executable,
                     "-m",
                     "gunicorn",
                     f"--bind={Url}",
                     *server_options,
                     flask_app,
                 ],
-                env={"TURNOVER_SETTINGS": fp.name},
+                env={"TURNOVER_SETTINGS": str(filename)},
                 prevent_sig=True,
             )
         if view_only:
             procs = [website]
         else:
             procs = [background, website]
```

### Comparing `protein_turnover-0.4.3/protein_turnover/web_ui.py` & `protein_turnover-0.4.4/protein_turnover/web_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.3/pyproject.toml` & `protein_turnover-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protein-turnover"
-version = "0.4.3"
+version = "0.4.4"
 description = "protein turnover pipeline"
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 license = "MIT"
 readme = "prerelease.md"
 exclude = ["oldcode/**", "tests/**"]
 packages = [{ include = "protein_turnover" }]
 repository = "https://github.com/arabidopsis/protein_turnover.git"
```

### Comparing `protein_turnover-0.4.3/PKG-INFO` & `protein_turnover-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-turnover
-Version: 0.4.3
+Version: 0.4.4
 Summary: protein turnover pipeline
 Home-page: https://github.com/arabidopsis/protein_turnover.git
 License: MIT
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
```

