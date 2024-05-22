# Comparing `tmp/protein_turnover-0.4.0.tar.gz` & `tmp/protein_turnover-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_turnover-0.4.0.tar", max compression
+gzip compressed data, was "protein_turnover-0.4.2.tar", max compression
```

## Comparing `protein_turnover-0.4.0.tar` & `protein_turnover-0.4.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.4.0/LICENSE
--rw-r--r--   0        0        0       54 2024-04-26 05:23:38.437576 protein_turnover-0.4.0/prerelease.md
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.4.0/protein_turnover/__init__.py
--rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.4.0/protein_turnover/__main__.py
--rw-r--r--   0        0        0      142 2024-04-18 09:07:07.364073 protein_turnover-0.4.0/protein_turnover/api.py
--rw-r--r--   0        0        0    11218 2024-05-17 13:48:47.050662 protein_turnover-0.4.0/protein_turnover/background.py
--rw-r--r--   0        0        0     1615 2024-05-17 03:46:28.509498 protein_turnover-0.4.0/protein_turnover/background_ui.py
--rw-r--r--   0        0        0     6670 2024-05-18 20:24:19.465998 protein_turnover-0.4.0/protein_turnover/broken_api.py
--rw-r--r--   0        0        0     2683 2024-05-19 06:28:47.088765 protein_turnover-0.4.0/protein_turnover/cli.py
--rw-r--r--   0        0        0     1086 2024-05-19 06:36:37.017269 protein_turnover-0.4.0/protein_turnover/config.py
--rw-r--r--   0        0        0     2439 2024-05-19 06:23:04.469379 protein_turnover-0.4.0/protein_turnover/config2.py
--rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.4.0/protein_turnover/dinosaur/__init__.py
--rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.4.0/protein_turnover/dinosaur/cmd.py
--rw-r--r--   0        0        0     1914 2024-05-19 04:54:45.120734 protein_turnover-0.4.0/protein_turnover/dinosaur/dinosaur.py
--rw-r--r--   0        0        0      393 2024-05-18 20:23:03.965361 protein_turnover-0.4.0/protein_turnover/exts.py
--rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.4.0/protein_turnover/filters.py
--rw-r--r--   0        0        0    19860 2024-05-17 22:50:45.333397 protein_turnover-0.4.0/protein_turnover/fitenvelopes.py
--rw-r--r--   0        0        0     8516 2024-05-17 11:31:30.621734 protein_turnover-0.4.0/protein_turnover/jobs.py
--rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.4.0/protein_turnover/logger.py
--rw-r--r--   0        0        0      981 2023-08-28 10:18:07.794829 protein_turnover-0.4.0/protein_turnover/mailer.py
--rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.4.0/protein_turnover/parallel_utils.py
--rw-r--r--   0        0        0    12689 2024-05-17 05:04:12.311778 protein_turnover-0.4.0/protein_turnover/pepxml.py
--rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.4.0/protein_turnover/pepxml_reader.py
--rw-r--r--   0        0        0    18506 2024-04-29 01:52:56.745780 protein_turnover-0.4.0/protein_turnover/plotting.py
--rw-r--r--   0        0        0     3826 2024-05-17 05:04:43.620071 protein_turnover-0.4.0/protein_turnover/protxml.py
--rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.4.0/protein_turnover/py.typed
--rw-r--r--   0        0        0    27261 2024-05-19 03:53:22.049512 protein_turnover-0.4.0/protein_turnover/pymz.py
--rw-r--r--   0        0        0    10895 2024-05-19 07:29:37.874358 protein_turnover-0.4.0/protein_turnover/pymz_ui.py
--rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.4.0/protein_turnover/settings.py
--rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.4.0/protein_turnover/sns.py
--rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.4.0/protein_turnover/sqla/__init__.py
--rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks.py
--rw-r--r--   0        0        0     3982 2024-04-12 09:19:03.622817 protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks_ui.py
--rw-r--r--   0        0        0    12901 2024-05-17 05:11:50.442492 protein_turnover-0.4.0/protein_turnover/sqla/model.py
--rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.4.0/protein_turnover/sqla/query.py
--rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.4.0/protein_turnover/sqla/utils.py
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.4.0/protein_turnover/types/__init__.py
--rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.4.0/protein_turnover/types/checking.py
--rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.4.0/protein_turnover/types/mzmltypes.py
--rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.4.0/protein_turnover/types/pepxmltypes.py
--rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.4.0/protein_turnover/types/turnovertype.py
--rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.4.0/protein_turnover/unimod.py
--rw-r--r--   0        0        0    21118 2024-05-18 20:30:54.981335 protein_turnover-0.4.0/protein_turnover/utils.py
--rw-r--r--   0        0        0     9788 2024-05-19 07:19:49.969162 protein_turnover-0.4.0/protein_turnover/web.py
--rw-r--r--   0        0        0     6383 2024-05-19 08:16:02.332675 protein_turnover-0.4.0/protein_turnover/web_ui.py
--rw-r--r--   0        0        0     1393 2024-05-19 09:00:24.475058 protein_turnover-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 protein_turnover-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.4.2/LICENSE
+-rw-r--r--   0        0        0       54 2024-05-20 06:25:28.823906 protein_turnover-0.4.2/prerelease.md
+-rw-r--r--   0        0        0    16384 2024-05-22 01:44:28.646339 protein_turnover-0.4.2/protein_turnover/.web.py.swp
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.4.2/protein_turnover/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.4.2/protein_turnover/__main__.py
+-rw-r--r--   0        0        0      140 2024-05-20 06:14:30.276214 protein_turnover-0.4.2/protein_turnover/api.py
+-rw-r--r--   0        0        0    11218 2024-05-17 13:48:47.050662 protein_turnover-0.4.2/protein_turnover/background.py
+-rw-r--r--   0        0        0     1619 2024-05-19 20:50:27.558491 protein_turnover-0.4.2/protein_turnover/background_ui.py
+-rw-r--r--   0        0        0     6670 2024-05-18 20:24:19.465998 protein_turnover-0.4.2/protein_turnover/broken_api.py
+-rw-r--r--   0        0        0     2706 2024-05-19 21:11:19.897073 protein_turnover-0.4.2/protein_turnover/cli.py
+-rw-r--r--   0        0        0     1120 2024-05-20 01:32:55.419976 protein_turnover-0.4.2/protein_turnover/config.py
+-rw-r--r--   0        0        0     2430 2024-05-20 01:32:50.255985 protein_turnover-0.4.2/protein_turnover/config2.py
+-rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.4.2/protein_turnover/dinosaur/__init__.py
+-rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.4.2/protein_turnover/dinosaur/cmd.py
+-rw-r--r--   0        0        0     1914 2024-05-19 04:54:45.120734 protein_turnover-0.4.2/protein_turnover/dinosaur/dinosaur.py
+-rw-r--r--   0        0        0      393 2024-05-18 20:23:03.965361 protein_turnover-0.4.2/protein_turnover/exts.py
+-rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.4.2/protein_turnover/filters.py
+-rw-r--r--   0        0        0    19857 2024-05-19 21:41:27.580566 protein_turnover-0.4.2/protein_turnover/fitenvelopes.py
+-rw-r--r--   0        0        0     8516 2024-05-17 11:31:30.621734 protein_turnover-0.4.2/protein_turnover/jobs.py
+-rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.4.2/protein_turnover/logger.py
+-rw-r--r--   0        0        0      979 2024-05-20 01:33:43.899913 protein_turnover-0.4.2/protein_turnover/mailer.py
+-rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.4.2/protein_turnover/parallel_utils.py
+-rw-r--r--   0        0        0    12689 2024-05-17 05:04:12.311778 protein_turnover-0.4.2/protein_turnover/pepxml.py
+-rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.4.2/protein_turnover/pepxml_reader.py
+-rw-r--r--   0        0        0    17519 2024-05-20 01:31:09.608194 protein_turnover-0.4.2/protein_turnover/plotting.py
+-rw-r--r--   0        0        0     3826 2024-05-17 05:04:43.620071 protein_turnover-0.4.2/protein_turnover/protxml.py
+-rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.4.2/protein_turnover/py.typed
+-rw-r--r--   0        0        0    27984 2024-05-20 06:17:31.161204 protein_turnover-0.4.2/protein_turnover/pymz.py
+-rw-r--r--   0        0        0    11026 2024-05-19 21:11:20.217076 protein_turnover-0.4.2/protein_turnover/pymz_ui.py
+-rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.4.2/protein_turnover/settings.py
+-rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.4.2/protein_turnover/sns.py
+-rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.4.2/protein_turnover/sqla/__init__.py
+-rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.4.2/protein_turnover/sqla/iso_peaks.py
+-rw-r--r--   0        0        0     4009 2024-05-19 21:11:19.197067 protein_turnover-0.4.2/protein_turnover/sqla/iso_peaks_ui.py
+-rw-r--r--   0        0        0    12901 2024-05-17 05:11:50.442492 protein_turnover-0.4.2/protein_turnover/sqla/model.py
+-rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.4.2/protein_turnover/sqla/query.py
+-rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.4.2/protein_turnover/sqla/utils.py
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.4.2/protein_turnover/types/__init__.py
+-rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.4.2/protein_turnover/types/checking.py
+-rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.4.2/protein_turnover/types/mzmltypes.py
+-rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.4.2/protein_turnover/types/pepxmltypes.py
+-rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.4.2/protein_turnover/types/turnovertype.py
+-rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.4.2/protein_turnover/unimod.py
+-rw-r--r--   0        0        0    21118 2024-05-18 20:30:54.981335 protein_turnover-0.4.2/protein_turnover/utils.py
+-rw-r--r--   0        0        0    10332 2024-05-22 02:27:01.163885 protein_turnover-0.4.2/protein_turnover/web.py
+-rw-r--r--   0        0        0     6393 2024-05-19 21:26:54.413011 protein_turnover-0.4.2/protein_turnover/web_ui.py
+-rw-r--r--   0        0        0     1484 2024-05-22 02:27:17.987986 protein_turnover-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 protein_turnover-0.4.2/PKG-INFO
```

### Comparing `protein_turnover-0.4.0/LICENSE` & `protein_turnover-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/background.py` & `protein_turnover-0.4.2/protein_turnover/background.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/background_ui.py` & `protein_turnover-0.4.2/protein_turnover/background_ui.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import click
 
 from .cli import cli
 from .cli import Config
 from .cli import pass_config
-from .logger import logger
 
 
 @cli.command(name="background")
 @click.option(
     "--workers",
     type=int,
     help="number of workers [default - half the number of cpus]",
@@ -52,14 +51,15 @@
     sleep: float,
     nice: int,
     no_email: bool = False,
 ) -> None:
     """Watch and run turnover jobs from directory"""
     from os import cpu_count
     from .background import SimpleQueue
+    from .logger import logger
 
     if workers is None:
         workers = max((cpu_count() or 1) // 2, 1)
         logger.warning("using %d workers", workers)
 
     squeue = SimpleQueue(
         directory,
```

### Comparing `protein_turnover-0.4.0/protein_turnover/broken_api.py` & `protein_turnover-0.4.2/protein_turnover/broken_api.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/cli.py` & `protein_turnover-0.4.2/protein_turnover/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
+import os
 from dataclasses import dataclass
 from pathlib import Path
 
 import click
 
 # from click_didyoumean import DYMGroup
 
-
+HIDDEN = os.environ.get("TURNOVER_FULL", "0") != "1"
 IsFile = click.Path(dir_okay=False, file_okay=True)
 
 CONFIG = Path("~/.turnover.toml").expanduser()
 
 
 @dataclass
 class Config:
@@ -48,25 +49,35 @@
         k = k.upper()
         if hasattr(config, k):
             setattr(config, k, v)
         else:
             click.secho(f"unknown configuration attribute {k}", fg="red")
 
 
-@click.group(epilog=click.style("turnover commands\n", fg="magenta"))
+epilog = click.style("turnover commands\n", fg="magenta")
+
+epilog = f"""{epilog}
+
+If no `--config` file is supplied `turnover` checks for a default configuration
+file at `~/.turnover.toml` (see `init-config` to make one).
+"""
+
+
+@click.group(epilog=epilog)
 @click.option(
     "-l",
     "--level",
     type=click.Choice(
         ["info", "debug", "warning", "error", "critical"],
         case_sensitive=False,
     ),
     help="log level",
 )
 @click.option(
+    "-f",
     "--logfile",
     type=click.Path(file_okay=True, dir_okay=False),
     help="log file to write to (use '-' to log to stderr)",
 )
 @click.option(
     "-m",
     "--mailhost",
@@ -86,22 +97,14 @@
     level: str | None,
     logfile: str | None = None,
     config: str | None = None,
     mailhost: str | None = None,
 ) -> None:
     from .logger import init_logger
 
-    # from .utils import df_can_write_parquet
-
-    # if not df_can_write_parquet():
-    #     click.secho(
-    #         "Please install pyarrow or fastparquet", fg="red", bold=True, err=True
-    #     )
-    #     raise click.Abort()
-
     ctx.obj = Config(
         logfile=logfile,
         loglevel=level,
         user_config=config,
     )
     if level is None:
         level = "WARNING"
```

### Comparing `protein_turnover-0.4.0/protein_turnover/config.py` & `protein_turnover-0.4.2/protein_turnover/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 
 MIN_RT = 2
 ABUNDANCE_CUTOFF = 0.01
 # split jobs into this many spectra
 # set to zero to not split
 NSPECTRA = 10000
 # quadrature limit for estimating area under curve (unused now)
-QUAD_LIMIT = 500
+# see USE_QUAD in fitenvelopes.py
+# QUAD_LIMIT = 500
 # https://docs.python.org/3/library/logging.html#logrecord-attributes
 LOG_FORMAT = "%(levelname)s|[%(asctime)s]|%(process)d| %(message)s"
 
 # XCMS_STEP = 0.0
 PEPXML_CHUNKS = 1000
 
 # also group on retention_time_sec
 GROUP_RT = False
 
-dpi = 96
-FIGSIZE = (1056.0 / dpi, 768.0 / dpi)
-
 MAIL_SUBJECT = "turnover pipeline"
 # default "from" sender
-MAIL_TURNOVER = "turnover-pipeline@uwa.edu.au"
+MAIL_SENDER = "turnover-pipeline@uwa.edu.au"
 # set to None or 'none' to stop any emailing
-MAIL_SERVER = "antivirus.uwa.edu.au"
+# e.g. MAIL_SERVER="uwa-edu-au.mail.protection.outlook.com"
+MAIL_SERVER = "mailhost"
 
 # e.g. "https://protein-turnover.plantenergy.org/inspect/{jobid}"
 INSPECT_URL: str | None = None
 # email template with {job:TurnoverJob, url:str}
 MAIL_TEXT = """Protein Turnover Job "{job.job_name}" has <b>finished</b>!{url}."""
 # set to True for production version (hides debug click commands)
```

### Comparing `protein_turnover-0.4.0/protein_turnover/config2.py` & `protein_turnover-0.4.2/protein_turnover/config2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 class TurnoverConfig:
     MIN_RT: int = 2
     ABUNDANCE_CUTOFF: float = 0.01
     # split jobs into this many spectra
     # set to zero to not split
     NSPECTRA: int = 10000
     # quadrature limit for estimating area under curve (unused now)
-    QUAD_LIMIT: int = 500
+    # QUAD_LIMIT: int = 500
     # https://docs.python.org/3/library/logging.html#logrecord-attributes
     LOG_FORMAT: str = "%(levelname)s|[%(asctime)s]|%(process)d| %(message)s"
 
     # XCMS_STEP = 0.0
     PEPXML_CHUNKS: int = 1000
 
     # also group on retention_time_sec
     GROUP_RT: bool = False
 
-    FIGSIZE: tuple[float, float] = (1056.0 / dpi, 768.0 / dpi)
+    # FIGSIZE: tuple[float, float] = (1056.0 / dpi, 768.0 / dpi)
 
     MAIL_SUBJECT: str = "turnover pipeline"
     # default "from" sender
-    MAIL_TURNOVER: str = "turnover-pipeline@uwa.edu.au"
+    MAIL_SENDER: str = "turnover-pipeline@uwa.edu.au"
     # set to None or 'none' to stop any emailing
-    MAIL_SERVER: str = "antivirus.uwa.edu.au"
+    MAIL_SERVER: str = "mailhost"
 
     # e.g. "https://protein-turnover.plantenergy.org/inspect/{jobid}"
     INSPECT_URL: str | None = None
     # email template with {job:TurnoverJob, url:str}
     MAIL_TEXT: str = (
         """Protein Turnover Job "{job.job_name}" has <b>finished</b>!{url}."""
     )
@@ -82,11 +82,12 @@
         return replace(config, **updates)
     return config
 
 
 def get_config() -> TurnoverConfig:
     return config
 
+
 def update_config(filename: str | Path) -> TurnoverConfig:
     global config
     config = _update_config(config, filename)
     return config
```

### Comparing `protein_turnover-0.4.0/protein_turnover/dinosaur/cmd.py` & `protein_turnover-0.4.2/protein_turnover/dinosaur/cmd.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/dinosaur/dinosaur.py` & `protein_turnover-0.4.2/protein_turnover/dinosaur/dinosaur.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/filters.py` & `protein_turnover-0.4.2/protein_turnover/filters.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/fitenvelopes.py` & `protein_turnover-0.4.2/protein_turnover/fitenvelopes.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 LOG_ERRORS = False
 
 R2 = np.sqrt(2.0).astype(np.float64)
 RPI2 = np.sqrt(np.pi / 2.0).astype(np.float64)
 NSIGMA = 2.0
 DELTA_ERF = (RPI2 * (erf(NSIGMA / R2) - erf(-NSIGMA / R2))).astype(np.float64)
 USE_QUAD = False
+QUAD_LIMIT = 500
 
 
 def fails(ival: int) -> str:
     return ", ".join(s for i, s in FAILS.items() if ival & (1 << i))
 
 
 @dataclass
@@ -291,15 +292,14 @@
 
 
 def fitIsotopeEnvelopes(
     peptide: str,
     rawEIC: np.ndarray,
 ) -> tuple[Envelope | None, int]:
     from .config import (
-        QUAD_LIMIT,
         INTERPOLATE_INTENSITY,
     )  # pylint: disable=import-outside-toplevel
 
     monoEIC: np.ndarray = rawEIC[1]
     rt, intensity = monoEIC[:, 0], monoEIC[:, 1]
     if INTERPOLATE_INTENSITY:
         # for fill_value='extrapolate'
```

### Comparing `protein_turnover-0.4.0/protein_turnover/jobs.py` & `protein_turnover-0.4.2/protein_turnover/jobs.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/logger.py` & `protein_turnover-0.4.2/protein_turnover/logger.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/mailer.py` & `protein_turnover-0.4.2/protein_turnover/mailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if mailhost is None or mailhost == "none":
         return False
 
     if subject is None:
         subject = config.MAIL_SUBJECT
 
     if me is None:
-        me = config.MAIL_TURNOVER
+        me = config.MAIL_SENDER
 
     msg = MIMEText(html, mimetype)
 
     msg["Subject"] = subject
     msg["From"] = me
     msg["To"] = you
     if replyto is not None:
```

### Comparing `protein_turnover-0.4.0/protein_turnover/parallel_utils.py` & `protein_turnover-0.4.2/protein_turnover/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/pepxml.py` & `protein_turnover-0.4.2/protein_turnover/pepxml.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/pepxml_reader.py` & `protein_turnover-0.4.2/protein_turnover/pepxml_reader.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/plotting.py` & `protein_turnover-0.4.2/protein_turnover/plotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from .types.turnovertype import TurnoverDict
 from .types.turnovertype import TurnoverRow
 from .utils import ensure_pos
 from .utils import isotopicDistribution
 from .utils import PeptideSettings
 from .utils import resize
 
+dpi = 96
+FIGSIZE: tuple[float, float] = (1056.0 / dpi, 768.0 / dpi)
 
 EICS_CMAP = plt.get_cmap("viridis")
 
 NEICS_CMAP = len(EICS_CMAP.colors)
 
 EIC_COLUMNS = ["peptide", "modcol", "eics", "eics_shape", "monoFitParams"]
 
@@ -42,30 +44,33 @@
     despine(ax=ax, bottom=True, trim=True)
 
 
 def despine_top(ax: Axes, offset: int = 5) -> None:
     despine(ax=ax, top=True, trim=True, offset=offset)
 
 
-def plotEICS(peptide: TurnoverRow, ax: Axes | None = None) -> Axes:
-    from .config import FIGSIZE
+def plotEICS(
+    peptide: TurnoverRow,
+    ax: Axes | None = None,
+    figsize: tuple[float, float] = FIGSIZE,
+) -> Axes:
     from .fitenvelopes import normalIntensityFunction, FAIL_W_CURVE
 
     pep = peptide.peptide
     mod = peptide.modcol
     eics = peptide.eics
     monoFitParams = peptide.monoFitParams
     fail = len(monoFitParams) == 0  # old way
     if hasattr(peptide, "fail"):  # my way
         fail = fail | (getattr(peptide, "fail") & (1 << FAIL_W_CURVE))
 
     # maxInt = eics[0,:, 1].max()
     # ylim = (0, maxInt)
     if ax is None:
-        fig = Figure(figsize=FIGSIZE)
+        fig = Figure(figsize=figsize)
         ax = fig.subplots()
     ax.set(xlabel="retention time", ylabel="Intensity", title=f"{pep} {mod}")
 
     m = eics[0]
     rt, im = m[:, 0], m[:, 1]
     ax.plot(rt, im, color="dodgerblue", lw=2)
     oeics = eics[2:]
@@ -111,20 +116,20 @@
 
 
 def plotLabelledEnvelope(
     peptide: TurnoverRow,
     settings: PeptideSettings,
     ax: Axes | None = None,
     scaled: bool = True,
+    figsize: tuple[float, float] = FIGSIZE,
 ) -> Axes:
-    from .config import FIGSIZE
     from .fitenvelopes import get_enrichments
 
     if ax is None:
-        fig = Figure(figsize=FIGSIZE)
+        fig = Figure(figsize=figsize)
         ax = fig.subplots()
     if len(peptide.labelledEnvelopes) > 0:
         e = peptide.labelledEnvelopes
         e = e if isinstance(e, np.ndarray) else np.array(e)
         x = intrange(len(e))
         enrichments = get_enrichments(peptide.peptide, settings)
         enrichments = resize(enrichments, len(e))
@@ -149,36 +154,14 @@
     ax.legend(labels=[peptide_legend(peptide)], handlelength=0)
     despine_bottom(ax)
     ax.xaxis.set_ticks_position("none")
     ax.set(title="labelledEnvelopes")
     return ax
 
 
-# def norm(peptide: TurnoverRow, settings: PeptideSettings):
-
-#     theoreticalDist = theoretical_dist(peptide.peptide, peptide.enrichment, settings)
-
-#     LPF = peptide.relativeIsotopeAbundance
-#     ndist = isotopicDistribution(peptide.peptide)
-#     naturalDist = ndist * (1 - LPF)
-#     labelledDist = theoreticalDist * LPF
-
-#     monoPeak = peptide.isotopeEnvelopes[1]
-#     denom = naturalDist[0] + labelledDist[0]
-#     fraction = 1.0 / denom if denom != 0 else np.inf
-#     scalingFactor = monoPeak * fraction
-
-#     naturalDist = resize(naturalDist, peptide.maxIso + 1)
-#     theoreticalDist = resize(labelledDist, peptide.maxIso + 1)
-#     # LPF == 0 => monoPeak * ndist/ndist[0]
-#     # LPF == 1 => monoPeak * ndist^A/ndist^A[0]
-#     # (theoreticalDist * scalingFactor)[0]  + (naturalDist * scalingFactor)[0] = monoPeak
-#     return theoreticalDist * scalingFactor, naturalDist * scalingFactor
-
-
 FITTED_COLUMNS = [
     "peptide",
     "modcol",
     "isotopeEnvelopes",
     "maxIso",
     "relativeIsotopeAbundance",
     "enrichment",
@@ -186,17 +169,16 @@
 ]
 
 
 def plotFittedEnvelopes(
     peptide: TurnoverRow,
     settings: PeptideSettings,
     ax: Axes | None = None,
+    figsize: tuple[float, float] = FIGSIZE,
 ) -> Axes:
-    from .config import FIGSIZE
-
     pep = peptide.peptide
     mod = peptide.modcol
     isotopeEnvelopes = peptide.isotopeEnvelopes
     if len(isotopeEnvelopes) == 0:
         logger.warning("plotFittedEnvelopes[%s]: no envelope!", pep)
         return ax
     has_adj = hasattr(peptide, "adjustedRsq")
@@ -212,15 +194,15 @@
     naturalDist = resize(naturalDist, peptide.maxIso + 1)
     theoreticalDist = resize(theoreticalDist, peptide.maxIso + 1)
 
     x = intrange(len(isotopeEnvelopes)) - 1
 
     heavyDistribution = ensure_pos(isotopeEnvelopes[1:] - naturalDist)
     if ax is None:
-        fig = Figure(figsize=FIGSIZE)
+        fig = Figure(figsize=figsize)
         ax = fig.subplots()
     xm1, x1 = x[:1], x[1:]  # skip negative heavy atom
     ax.set(title=f"{pep} {mod}")
     ax.bar(
         x1,
         isotopeEnvelopes[1:],
         color="turquoise",
@@ -251,29 +233,28 @@
     return ax
 
 
 def plotIntensities(
     peptide: TurnoverRow,  # eics
     eici: list[int] | None = None,
     ax: Axes | None = None,
-    figsize: tuple[float, float] | None = None,
+    figsize: tuple[float, float] = FIGSIZE,
 ) -> Axes:
     from scipy.linalg import lstsq
-    from .config import FIGSIZE
 
     intensity = peptide.eics[1, :, 1]
     im = np.c_[np.ones(len(intensity)), intensity]
     x = np.linspace(np.min(intensity), np.max(intensity), num=30)
     idx = set(range(peptide.eics.shape[0]))
     if eici is None:
         eici = list(idx)
     else:
         eici = list(sorted(set(eici) & idx))
     if ax is None:
-        fig = Figure(figsize=figsize if figsize else FIGSIZE)
+        fig = Figure(figsize=figsize)
         ax = fig.subplots(1, 1)
     for i in eici:
         ints = peptide.eics[i, :, 1]
         fit, _residues, _rank, _s = lstsq(im, ints)
 
         y = fit[0] + fit[1] * x
         ax.scatter(intensity, ints, s=10)
@@ -289,16 +270,14 @@
 def enrichment_plot(
     turn: pd.DataFrame,
     factor: float = 2.0,
     ax: Axes | None = None,
     figsize: tuple[float, float] | None = None,
     column: str = "enrichment",
 ) -> Axes:
-    from .config import FIGSIZE
-
     enrich = turn[column]
     enrich = enrich[enrich.notna()]
     em = enrich.mean()
     esd = enrich.std()
     if ax is None:
         fig = Figure(figsize=figsize if figsize else FIGSIZE)
         ax = fig.subplots(1, 1)
@@ -342,16 +321,14 @@
 
 def nnls_plot(
     df: pd.DataFrame,
     ax: Axes | None = None,
     figsize: tuple[float, float] | None = None,
     percent: float = 0.01,
 ) -> Axes:
-    from .config import FIGSIZE
-
     nnls = nnls_values(df, percent=percent)
 
     if ax is None:
         fig = Figure(figsize=figsize if figsize else FIGSIZE)
         ax = fig.subplots(1, 1)
     # mn,mx = nnls_residual.min(), nnls_residual.max()
     ax.hist(nnls, bins="auto", color="turquoise")
@@ -363,16 +340,14 @@
 def correlation_plot(
     df: pd.DataFrame,
     column: str,
     xlabel: str | None = None,
     ax: Axes | None = None,
     figsize: tuple[float, float] | None = None,
 ) -> Axes:
-    from .config import FIGSIZE
-
     if ax is None:
         fig = Figure(figsize=figsize if figsize else FIGSIZE)
         ax = fig.subplots(1, 1)
     # mn,mx = nnls_residual.min(), nnls_residual.max()
     col = df[column]
     ax.hist(col, bins="auto", color="turquoise")
     despine(ax, trim=True, offset=5)
@@ -386,16 +361,14 @@
 def plot_all(
     peptide: TurnoverRow,
     settings: PeptideSettings,
     figsize: tuple[float, float] | None = None,
     hspace: float = 0.5,
     portrait: bool = True,
 ) -> tuple[Figure, list[Axes]]:
-    from .config import FIGSIZE
-
     if figsize is None:
         figsize = FIGSIZE[0], 3 * FIGSIZE[1]
 
     if not portrait:
         r, c = 1, 3
     else:
         r, c = 3, 1
```

### Comparing `protein_turnover-0.4.0/protein_turnover/protxml.py` & `protein_turnover-0.4.2/protein_turnover/protxml.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/pymz.py` & `protein_turnover-0.4.2/protein_turnover/pymz.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dataclasses import asdict
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Iterator
 from typing import NamedTuple
+from typing import overload
 from typing import TypedDict
 
 import numpy as np
 import pandas as pd
 
 from .fitenvelopes import fitEnvelopes
 from .jobs import TurnoverJob
@@ -75,21 +76,21 @@
 def mzi_max_intensity(mzi: np.ndarray, mzmin: float, mzmax: float) -> float:
     mz, i = mzi[0], mzi[1]
     q = (mz <= mzmax) & (mz >= mzmin)
     return i[q].max() if q.any() else 0.0
 
 
 def zeroi() -> np.ndarray:
-    return np.array([], dtype=np.float32).reshape(MzML.SHAPE)
+    return np.array([], dtype=np.float32).reshape(MZI.SHAPE)
 
 
 COLS = ("mzmin", "mzmax", "rtmin", "rtmax")
 
 
-class MzML:
+class MZI:
     SHAPE = (2, -1)
 
     def __init__(
         self,
         mzmlfile: MzMLResourceFile,
     ):
         self.name = mzmlfile.name
@@ -97,15 +98,15 @@
 
         self._mzi = np.memmap(mapname, dtype=np.float32, mode="r")
 
         if self._mzi[0] != MAGIC_NO:
             raise ByteOrderError(
                 f'file "{mapname}" can\'t be read (written with different byteorder)',
             )
-
+        # columns: retention_time_sec', 'scanindex', 'mzmax', 'mzmin', 'imax'
         self.df = IO(meta).read_df()
 
         scanstart = np.concatenate(  # pylint: disable=unexpected-keyword-arg
             ([1], self.df["scanindex"].to_numpy(dtype=np.int64)[:-1]),
             dtype=np.int64,
         )
         self.df["scanstart"] = scanstart
@@ -120,15 +121,15 @@
         # if dino.exists():
         #     self.dino = IO(dino).read_df(columns=["mz", "rtStart", "rtEnd"])
         # else:
         #     self.dino = None
 
     def __repr__(self) -> str:
         return (
-            f"MzML({self.name}[{len(self.df)}],"
+            f"MZI({self.name}[{len(self.df)}],"
             f" mz=[{self.search.mzmin:.2f},{self.search.mzmax:.2f}],"
             f" rt=[{self.search.rtmin:.2f},{self.search.rtmax:.2f}])"
         )
 
     def mzi_column(self, df: pd.DataFrame | None = None) -> pd.Series:
         if df is None:
             df = self.df
@@ -137,19 +138,19 @@
     def mzi(self, scanstart: int, scanindex: int) -> np.ndarray:
         return self._mzi[scanstart:scanindex].reshape(self.SHAPE)
 
     def mzi_apply(self, row: pd.Series) -> np.ndarray:
         return self.mzi(row["scanstart"], row["scanindex"])
 
     @classmethod
-    def from_path(cls, path: str) -> MzML:
+    def from_path(cls, path: str) -> MZI:
         return cls(MzMLResourceFile(path))
 
     @classmethod
-    def from_file(cls, mzmlfile: str, directory: str | None = None) -> MzML:
+    def from_file(cls, mzmlfile: str, directory: str | None = None) -> MZI:
         return cls(MzMLResourceFileLocal(mzmlfile, directory))
 
     @classmethod
     def can_read_mzi(cls, mzi: str | Path) -> bool:
         _mzi = np.memmap(mzi, dtype=np.float32, mode="r")
         return _mzi[0] == MAGIC_NO
 
@@ -260,14 +261,37 @@
 
     @classmethod
     def rehydrate_eics(cls, s: pd.Series) -> pd.Series:
         return s.apply(
             lambda a: a.reshape(cls.SHAPE) if isinstance(a, np.ndarray) else a,
         )
 
+    def __len__(self) -> int:
+        return len(self.df)
+
+    @overload
+    def __getitem__(self, idx: int) -> np.ndarray:
+        ...
+
+    @overload
+    def __getitem__(self, idx: slice) -> pd.Series:
+        ...
+
+    @overload
+    def __getitem__(self, idx: list[int]) -> pd.Series:
+        ...
+
+    def __getitem__(self, idx: int | list[int] | slice) -> np.ndarray | pd.Series:
+        df = self.df[["scanstart", "scanindex"]].iloc[idx]
+        if isinstance(idx, int):
+            scanstart, scanindex = df
+            return self.mzi(scanstart, scanindex)
+
+        return df.apply(self.mzi_apply, axis=1)  # .to_numpy()
+
 
 # number must survive roundtrip....
 # struct.unpack("f", struct.pack("f", MAGIC_NO))[0] == MAGIC_NO
 MAGIC_NO = -0.1234000027179718
 # MAGIC_BYTES = b'$\xb9\xfc\xbd'
 MAGIC_BYTES = np.array([MAGIC_NO], dtype=np.float32).tobytes()
 
@@ -569,15 +593,15 @@
             )
 
     return ret
 
 
 class MzMLTask(Task):
     def task_run(self) -> pd.DataFrame:
-        mzmlc = MzML(self.mzml)
+        mzmlc = MZI(self.mzml)
         done = mzml_calc_mzml_envelopes(
             self.pepxml_df,
             mzmlc,
             self.settings,
             level=self.level,
             number_of_bg_processes=self.number_of_bg_processes,
         )
@@ -634,15 +658,15 @@
     ]
 
     return tasks
 
 
 def calc_rtranges(
     rundf: pd.DataFrame,
-    mzmlc: MzML,
+    mzmlc: MZI,
     settings: PeptideSettings,
     rt_min: int,
 ) -> pd.DataFrame:
     rt = mzmlc.df["retention_time_sec"]
     if mzmlc.dino is not None:
         rundf = rundf.join(findrt_dino(mzmlc.dino, rundf, rt, settings))
         rrt = rundf.rtmax - rundf.rtmin
@@ -731,15 +755,15 @@
         findrtrange,
         axis=1,
     )
 
 
 def mzml_calc_mzml_envelopes(
     rundf: pd.DataFrame,
-    mzmlc: MzML,
+    mzmlc: MZI,
     settings: PeptideSettings,
     level: int = 0,
     number_of_bg_processes: int = 1,
 ) -> list[dict[str, Any]]:
     from .logger import log_iterator
     from .config import MIN_RT
 
@@ -787,15 +811,15 @@
         len(done),
         total,
     )
     return done
 
 
 def mzml_calc_pep_envelopes(
-    mzmlc: MzML,
+    mzmlc: MZI,
     row: PepXMLRunRowRT,
     settings: PeptideSettings,
 ) -> dict[str, Any] | None:
     from .config import MIN_RT
 
     rtmin, rtmax = row.rtmin, row.rtmax
```

### Comparing `protein_turnover-0.4.0/protein_turnover/pymz_ui.py` & `protein_turnover-0.4.2/protein_turnover/pymz_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Callable
+from typing import TYPE_CHECKING
 
 import click
 
 from .cli import cli
 from .cli import Config
 from .cli import IsFile
 from .cli import pass_config
-from .jobs import slugify
-from .logger import logger
 from .settings import setting_options
-from .utils import PeptideSettings
+
+if TYPE_CHECKING:
+    from .utils import PeptideSettings
 
 
 @cli.command(name="mzi-create", hidden=False)
 @click.option("--force", is_flag=True, help="force creation")
 @click.option(
     "-w",
     "--workers",
@@ -40,14 +41,15 @@
 
     from functools import partial
     from os import cpu_count
 
     from .utils import MzMLResourceFileLocal
     from .parallel_utils import parallel_result
     from .pymz import mzml_create
+    from .logger import logger
 
     if workers is None:
         workers = max((cpu_count() or 1) // 2, 1)
 
     targets = [MzMLResourceFileLocal(m, out) for m in set(mzmlfiles)]
     todo = [t for t in targets if not t.cache_mzml_ok()] if not force else targets
     skipped = set(targets) - set(todo)
@@ -74,30 +76,34 @@
 @cli.command(name="run")
 @click.option(
     "-w",
     "--workers",
     type=int,
     help="number of parallel workers [default: half the number of cpus]",
 )
-@click.option("--nspectra", type=int, help="split tasks into this many spectra")
+@click.option(
+    "--nspectra",
+    type=int,
+    help="split tasks into this many spectra (see NSPECTRA configuration variable)",
+)
 @click.option(
     "--job-dir",
     type=click.Path(file_okay=False),
     help="directory to run job [default: directory of jobfile]",
 )
 @click.option(
     "--cache-dir",
     type=click.Path(file_okay=False),
     help="directory to store cache files [default: cache_dir specified in jobfile]",
 )
 @click.option("--force", is_flag=True, help="force (re)creation of cache files")
 @click.option(
     "--no-email",
     is_flag=True,
-    help="don't send any emails",
+    help="don't send any emails when finished",
 )  # see runner.py
 @click.option(
     "--interrupt-as-error",
     default=0,
     help="accept keyboard interrupt as error. Value will be exit code",
     hidden=True,  # only useful to for background process: see runner.py
 )  # see runner.py
@@ -243,14 +249,15 @@
     out: str | None = None,
 ) -> None:
     """Create a turnover job file"""
     from .jobs import TurnoverJob, jobidkey
     from .pepxml import scan_spectra
     from .protxml import scan_proteins
     from .pymz import scan_mzml_spectra
+    from .jobs import slugify
 
     if not no_check:
         missing = []
         for f in [pepxml, protxml, *mzmlfiles]:
             if not Path(f).exists():
                 missing.append(f)
         if missing:
```

### Comparing `protein_turnover-0.4.0/protein_turnover/settings.py` & `protein_turnover-0.4.2/protein_turnover/settings.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/sns.py` & `protein_turnover-0.4.2/protein_turnover/sns.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks.py` & `protein_turnover-0.4.2/protein_turnover/sqla/iso_peaks.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/sqla/iso_peaks_ui.py` & `protein_turnover-0.4.2/protein_turnover/sqla/iso_peaks_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import click
 
 from ..cli import cli
+from ..cli import HIDDEN
 
 
-@cli.group(help=click.style("add sqlite columns", fg="magenta"), hidden=True)
+@cli.group(help=click.style("add sqlite columns", fg="magenta"), hidden=HIDDEN)
 def fix() -> None:
     pass
 
 
 def show(filename: str, *, echo: bool = False):
     from .model import file2engine
     from .model import Peptide
```

### Comparing `protein_turnover-0.4.0/protein_turnover/sqla/model.py` & `protein_turnover-0.4.2/protein_turnover/sqla/model.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/sqla/query.py` & `protein_turnover-0.4.2/protein_turnover/sqla/query.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/sqla/utils.py` & `protein_turnover-0.4.2/protein_turnover/sqla/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/types/checking.py` & `protein_turnover-0.4.2/protein_turnover/types/checking.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/types/mzmltypes.py` & `protein_turnover-0.4.2/protein_turnover/types/mzmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/types/pepxmltypes.py` & `protein_turnover-0.4.2/protein_turnover/types/pepxmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/types/turnovertype.py` & `protein_turnover-0.4.2/protein_turnover/types/turnovertype.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/unimod.py` & `protein_turnover-0.4.2/protein_turnover/unimod.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/utils.py` & `protein_turnover-0.4.2/protein_turnover/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.4.0/protein_turnover/web.py` & `protein_turnover-0.4.2/protein_turnover/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import tomli as tomllib
 import tomli_w
 from typing_extensions import NotRequired
 
 from .background import Processing
 from .cli import CONFIG
 
+IS_WIN32 = sys.platform == "win32"
 
 # def dict2conf(outfile: str, dictionary: dict[str, Any]) -> None:
 
 #     with open(outfile, mode="wb") as fp:
 #         tomli_w.dump(dictionary, fp)
 
 
@@ -44,15 +45,15 @@
 
 @dataclass
 class Runner:
     name: str
     cmd: list[str]
     directory: str = "."
     env: dict[str, str] | None = None
-    showcmd: bool = False
+    showcmd: bool = True
     shell: bool = False
     prevent_sig: bool = False  # prevent Cntrl-C from propagating to child process
 
     def getenv(self) -> dict[str, str] | None:
         if not self.env:
             return None
         return {**os.environ, **self.env}
@@ -63,24 +64,26 @@
 
         kwargs = PopenArgs(creationflags=0, preexec_fn=None)
         if self.prevent_sig:
             if sys.platform == "win32":
                 kwargs["creationflags"] = (
                     subprocess.DETACHED_PROCESS | subprocess.CREATE_NEW_PROCESS_GROUP
                 )
+                shell = True
             else:
+                shell = self.shell
                 if sys.version_info >= (3, 11):
                     kwargs["process_group"] = 0
                 else:
                     kwargs["preexec_fn"] = os.setpgrp
         return subprocess.Popen(  # type: ignore
             self.cmd,
             cwd=self.directory,
             env=self.getenv(),
-            shell=self.shell,
+            shell=shell,
             **kwargs,
         )
 
 
 def browser(url: str = "http://127.0.0.1:8000", sleep: float = 5.0) -> Thread:
     import webbrowser
 
@@ -132,17 +135,16 @@
     # conf = Config(".")
     # conf.from_pyfile(config)
     # return conf
     try:
         with open(config, "rb") as fp:
             ret = tomllib.load(fp)
             if ns is not None:
-                ret2 = ret.get(ns)
-                if isinstance(ret2, dict):
-                    return ret2
+                ret2 = ret.get(ns, None)
+                return ret2 or {}
             return ret
     except tomllib.TOMLDecodeError as e:
         raise click.BadParameter(f'Can\'t read configuration file "{config}"') from e
 
 
 def dump_config(configfile: Path, with_website: bool):
     from . import config
@@ -175,15 +177,15 @@
         tomli_w.dump(d, fp)
 
 
 def webrunner(
     *,
     browse: bool,
     workers: int,
-    web_config: str | Path | None = None,  # ~/.turnover-web.toml or commandline
+    web_config: str | Path | None = None,  # from --web-config
     gunicorn: bool = False,
     view_only: bool = True,
     configfile: str | None = None,  # turnover config file
     defaults: dict[str, Any] | None = None,  # CACHEDIR etc. from commanline
     port: int = 8000,
     server_options: tuple[str, ...] = (),  # extra commandline arguments after --
     flask_app: str = "protein_turnover_website.wsgi",
@@ -285,26 +287,37 @@
                 env={"TURNOVER_SETTINGS": fp.name},
                 prevent_sig=True,
             )
         if view_only:
             procs = [website]
         else:
             procs = [background, website]
-        # handler = InterruptHandler()
+
         processes = [(p.name, p.start()) for p in procs]
 
         if browse:
             browser(url=f"http://{Url}", sleep=3.0)
 
         worker = Processing(jobsdir)
         ninterrupts = 0
         prev = datetime.now()
         while True:
             try:
-                time.sleep(100.0)
+                time.sleep(10.0)
+                failed = False
+                for n, tr in processes:
+                    try:
+                        retcode = tr.wait(1.0)
+                        if retcode != 0:
+                            click.echo(f"process failed {n}")
+                            failed = True
+                    except subprocess.TimeoutExpired:
+                        pass
+                if failed:
+                    raise KeyboardInterrupt()
 
             except KeyboardInterrupt:
                 # too long between ^C
                 now = datetime.now()
                 if (
                     ninterrupts > 0
                     and not view_only
@@ -313,15 +326,17 @@
                     ninterrupts = 0
                     prev = now
                     continue
                 ninterrupts += 1
                 if ninterrupts >= 2 or view_only:
                     for name, tr in processes:
                         click.secho(f"terminating... {name}", fg="blue")
-                        tr.send_signal(signal.SIGINT)
+                        tr.send_signal(
+                            signal.SIGINT if not IS_WIN32 else signal.CTRL_BREAK_EVENT
+                        )
 
                     for name, tr in processes:
                         try:
                             tr.wait(timeout=4.0)
                         except (OSError, subprocess.TimeoutExpired):
                             pass
                     sys.exit(os.EX_OK)
```

### Comparing `protein_turnover-0.4.0/protein_turnover/web_ui.py` & `protein_turnover-0.4.2/protein_turnover/web_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 )
 @click.option(
     "--cache-dir",
     type=click.Path(file_okay=False),
     help="directory to store file caches [default: directory of ~/turnover_cache]",
 )
 @click.option(
+    "-v",
     "--view-only",
     is_flag=True,
     help="only view data",
 )
 @click.option(
     "--email",
     is_flag=True,
```

### Comparing `protein_turnover-0.4.0/pyproject.toml` & `protein_turnover-0.4.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protein-turnover"
-version = "0.4.0"
+version = "0.4.2"
 description = "protein turnover pipeline"
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 license = "MIT"
 readme = "prerelease.md"
 exclude = ["oldcode/**", "tests/**"]
 packages = [{ include = "protein_turnover" }]
 repository = "https://github.com/arabidopsis/protein_turnover.git"
@@ -18,18 +18,18 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 pymzml = "^2.5.2"
 pyteomics = "^4.5.3"
 lxml = "^4.9.0"
 click = "^8.1.3"
-scipy = "^1.8.1"  # for fitting
+scipy = "^1.8.1"                                    # for fitting
 pandas = "^2.0.3"
-pyarrow = "^15.0.0" # for parquet
-more-itertools = "^8.13.0" # ichunked
+pyarrow = "^15.0.0"                                 # for parquet
+more-itertools = "^8.13.0"                          # ichunked
 matplotlib = "^3.5.2"
 SQLAlchemy = "^2.0.20"
 tomli = "^2.0.1"
 tomli-w = "^1.0.0"
 unidecode = { version = "^1.3.8", optional = true }
 psutil = { version = "^5.0", optional = true }
```

### Comparing `protein_turnover-0.4.0/PKG-INFO` & `protein_turnover-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-turnover
-Version: 0.4.0
+Version: 0.4.2
 Summary: protein turnover pipeline
 Home-page: https://github.com/arabidopsis/protein_turnover.git
 License: MIT
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
```

