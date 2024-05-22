# Comparing `tmp/nomad_tools-0.3.1.tar.gz` & `tmp/nomad_tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_tools-0.3.1.tar", last modified: Sun Apr 28 10:40:13 2024, max compression
+gzip compressed data, was "nomad_tools-0.3.2.tar", last modified: Wed May 22 09:16:16 2024, max compression
```

## Comparing `nomad_tools-0.3.1.tar` & `nomad_tools-0.3.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.526031 nomad_tools-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-28 10:40:13.526031 nomad_tools-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:40:13.526031 nomad_tools-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.518031 nomad_tools-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/common_nomad.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/entry_constrainteval.py
--rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/entry_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/exit_on_thread_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/flagdebug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28872 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_dockers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_downloadrelease.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/script.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/waiter.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    28600 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_smart_start_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_taskexec.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18624 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_vardir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77612 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomad_watch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomaddbjob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools/nomadlib/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/datadict.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadlib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/nomadt_completion.sh
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/taskexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/src/nomad_tools/transferstats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/src/nomad_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 10:40:13.000000 nomad_tools-0.3.1/src/nomad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:40:13.522031 nomad_tools-0.3.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/tests/test_nomad_cp_complete.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/tests/test_taskexec_transfer_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-28 10:40:05.000000 nomad_tools-0.3.1/tests/testlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:16.536656 nomad_tools-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-05-22 09:16:16.536656 nomad_tools-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:16:16.540656 nomad_tools-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:16.528656 nomad_tools-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:16.536656 nomad_tools-0.3.2/src/nomad_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/common_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/common_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/common_nomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/entry_constrainteval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/entry_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/exit_on_thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/flagdebug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28872 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_dockers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_downloadrelease.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:16.536656 nomad_tools-0.3.2/src/nomad_tools/nomad_gitlab_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_gitlab_runner/script.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_gitlab_runner/waiter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28600 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_gitlab_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_smart_start_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_taskexec.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18624 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_vardir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    78146 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomad_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomaddbjob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:16.536656 nomad_tools-0.3.2/src/nomad_tools/nomadlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomadlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomadlib/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomadlib/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomadlib/datadict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomadlib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomadlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/nomadt_completion.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/taskexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/src/nomad_tools/transferstats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:16.536656 nomad_tools-0.3.2/src/nomad_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-05-22 09:16:16.000000 nomad_tools-0.3.2/src/nomad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-22 09:16:16.000000 nomad_tools-0.3.2/src/nomad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:16:16.000000 nomad_tools-0.3.2/src/nomad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 09:16:16.000000 nomad_tools-0.3.2/src/nomad_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-22 09:16:16.000000 nomad_tools-0.3.2/src/nomad_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 09:16:16.000000 nomad_tools-0.3.2/src/nomad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:16:16.536656 nomad_tools-0.3.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/tests/test_nomad_cp_complete.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/tests/test_taskexec_transfer_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-05-22 09:16:09.000000 nomad_tools-0.3.2/tests/testlib.py
```

### Comparing `nomad_tools-0.3.1/LICENSE` & `nomad_tools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/PKG-INFO` & `nomad_tools-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: Set of tools and utilities to ease interacting with Hashicorp Nomad scheduling solution.
 Author: Kamil Cukrowski
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/Kamilcuk/nomad-tools
 Project-URL: repository, https://github.com/Kamilcuk/nomad-tools
 Project-URL: documentation, https://github.com/Kamilcuk/nomad-tools
 Description-Content-Type: text/markdown
```

### Comparing `nomad_tools-0.3.1/README.md` & `nomad_tools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/pyproject.toml` & `nomad_tools-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/colors.py` & `nomad_tools-0.3.2/src/nomad_tools/colors.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/common_base.py` & `nomad_tools-0.3.2/src/nomad_tools/common_base.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/common_click.py` & `nomad_tools-0.3.2/src/nomad_tools/common_click.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/common_nomad.py` & `nomad_tools-0.3.2/src/nomad_tools/common_nomad.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/entry_constrainteval.py` & `nomad_tools-0.3.2/src/nomad_tools/entry_constrainteval.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/entry_go.py` & `nomad_tools-0.3.2/src/nomad_tools/entry_go.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/entrypoint.py` & `nomad_tools-0.3.2/src/nomad_tools/entrypoint.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/exit_on_thread_exception.py` & `nomad_tools-0.3.2/src/nomad_tools/exit_on_thread_exception.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/flagdebug.py` & `nomad_tools-0.3.2/src/nomad_tools/flagdebug.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_cp.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_cp.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_dockers.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_dockers.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_downloadrelease.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_downloadrelease.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/script.sh` & `nomad_tools-0.3.2/src/nomad_tools/nomad_gitlab_runner/script.sh`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner/waiter.sh` & `nomad_tools-0.3.2/src/nomad_tools/nomad_gitlab_runner/waiter.sh`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_gitlab_runner.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_port.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_port.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_smart_start_job.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_smart_start_job.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_taskexec.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_taskexec.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_vardir.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_vardir.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomad_watch.py` & `nomad_tools-0.3.2/src/nomad_tools/nomad_watch.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,15 +653,15 @@
             for event in self.read_json_stream(stream):
                 if event:
                     line64: Optional[str] = event.get("Data")
                     if line64:
                         linebytes = base64.b64decode(line64.encode())
                         lines = linebytes.decode(errors="replace").splitlines()
                         for line in lines:
-                            self.tk.log_task(self.stderr, line.strip())
+                            self.tk.log_task(self.stderr, line.rstrip())
                     fileevent: Optional[str] = event.get("FileEvent")
                     if fileevent == "file deleted":
                         # Deleted means end of stream.
                         break
                 # Nomad json stream every second sends empty {}.
                 # If requested to exit, then exit.
                 if self.exitreqtime is not None:
@@ -969,15 +969,15 @@
 
 
 ###############################################################################
 
 
 def __nomad_job_run(args: List[str]) -> str:
     """Call nomad job run to start a Nomad job using nomad job run call with specified arguments"""
-    cmd: List[str] = "nomad job run -detach -verbose".split() + args
+    cmd: List[str] = [*"nomad job run -detach -verbose".split(), *args]
     log.info(f"+ {' '.join(shlex.quote(x) for x in cmd)}")
     try:
         output = subprocess.check_output(cmd, text=True, stdin=sys.stdin)
     except subprocess.CalledProcessError as e:
         # nomad will print its error, we can just exit
         exit(e.returncode)
     # Extract evaluation id from Nomad output.
@@ -1930,15 +1930,15 @@
 
 cli_jobid = click.argument(
     "jobid",
     shell_complete=complete_job(),
 )
 
 
-def cli_jobfile(name: str, help: str):
+def cli_jobfile_disabled(name: str, help: str):
     # Disabled, because maintenance.
     nomad_job_run_flags = [
         click.option("-check-index", type=int),
         click.option("-detach", is_flag=True),
         click.option("-eval-priority", type=int),
         click.option("-json", is_flag=True),
         click.option("-hcl1", is_flag=True),
@@ -1965,24 +1965,24 @@
         click.argument(
             "jobfile",
             shell_complete=click.File().shell_complete,
         ),
     )
 
 
-def cli_command_run_nomad_job_run(name: str, help: str):
-    """Command that forwards all arguments to 'nomad job run' command."""
+def cli_jobfile_command(name: str, where: str, help: str):
+    f"""Command that forwards all arguments to 'nomad job {where}' command."""
     return composed(
         cli.command(
             name,
             help=help.rstrip()
-            + """
+            + f"""
 
-            All following arguments are forwarded to 'nomad job run' command.
-            Note that 'nomad job run' has arguments starting with a single dash.
+            All following arguments are forwarded to 'nomad {where}' command.
+            Note that 'nomad job {where}' has arguments starting with a single dash.
             """,
             context_settings=dict(ignore_unknown_options=True),
         ),
         click.argument(
             "args",
             nargs=-1,
             shell_complete=click.File().shell_complete,
@@ -2025,37 +2025,38 @@
 def mode_eval(evalid):
     evaluation = mynomad.get("evaluations", params={"prefix": evalid})
     assert len(evaluation) > 0, f"Evaluation with id {evalid} not found"
     assert len(evaluation) < 2, f"Multiple evaluations found starting with id {evalid}"
     NomadJobWatcherUntilFinished(None, nomadlib.Eval(evaluation[0])).run_and_exit()
 
 
-@cli_command_run_nomad_job_run(
+@cli_jobfile_command(
+    "run",
     "run",
     help="Run a Nomad job and then act like stopped mode.",
 )
-def mode_run(args: Tuple[str], jobfile: str):
+def mode_run(args: Tuple[str, ...], jobfile: str):
     evaluation = nomad_start_job(list(args) + [jobfile])
     NomadJobWatcherUntilFinished(None, evaluation).run_and_exit()
 
 
 @cli.command(
     "job",
     help="Alias to stopped command.",
 )
 @cli_jobid
 def mode_job(jobid: str):
     jobid = nomad_find_job(jobid)
     NomadJobWatcherUntilFinished(jobid).run_and_exit()
 
 
-@cli_command_run_nomad_job_run(
-    "start", help="Start a Nomad job file and then act like started command."
+@cli_jobfile_command(
+    "start", "run", help="Start a Nomad job file and then act like started command."
 )
-def mode_start(args: Tuple[str], jobfile: str):
+def mode_start(args: Tuple[str, ...], jobfile: str):
     evaluation = nomad_start_job(list(args) + [jobfile])
     NomadJobWatcherUntilStarted(None, evaluation).run_and_exit()
 
 
 @cli.command(
     "started",
     help=f"""
@@ -2148,11 +2149,28 @@
 )
 @cli_jobid
 def mode_stopped(jobid: str):
     jobid = nomad_find_job(jobid)
     NomadJobWatcherUntilFinished(jobid).run_and_exit()
 
 
+@cli_jobfile_command(
+    "plan",
+    "plan",
+    help=f"""
+    This is an alias to nomad job plan for ease of typing.
+    """,
+)
+def mode_plan(args: Tuple[str, ...], jobfile: str):
+    cmd: List[str] = [*"nomad job plan".split(), *args, jobfile]
+    log.info(f"+ {' '.join(shlex.quote(x) for x in cmd)}")
+    try:
+        output = subprocess.check_call(cmd, text=True)
+    except subprocess.CalledProcessError as e:
+        # nomad will print its error, we can just exit
+        exit(e.returncode)
+
+
 ###############################################################################
 
 if __name__ == "__main__":
     cli.main()
```

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomaddbjob.py` & `nomad_tools-0.3.2/src/nomad_tools/nomaddbjob.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomadlib/_generator.py` & `nomad_tools-0.3.2/src/nomad_tools/nomadlib/_generator.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomadlib/connection.py` & `nomad_tools-0.3.2/src/nomad_tools/nomadlib/connection.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomadlib/datadict.py` & `nomad_tools-0.3.2/src/nomad_tools/nomadlib/datadict.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomadlib/tools.py` & `nomad_tools-0.3.2/src/nomad_tools/nomadlib/tools.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomadlib/types.py` & `nomad_tools-0.3.2/src/nomad_tools/nomadlib/types.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/nomadt_completion.sh` & `nomad_tools-0.3.2/src/nomad_tools/nomadt_completion.sh`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/taskexec.py` & `nomad_tools-0.3.2/src/nomad_tools/taskexec.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools/transferstats.py` & `nomad_tools-0.3.2/src/nomad_tools/transferstats.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/src/nomad_tools.egg-info/PKG-INFO` & `nomad_tools-0.3.2/src/nomad_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: Set of tools and utilities to ease interacting with Hashicorp Nomad scheduling solution.
 Author: Kamil Cukrowski
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/Kamilcuk/nomad-tools
 Project-URL: repository, https://github.com/Kamilcuk/nomad-tools
 Project-URL: documentation, https://github.com/Kamilcuk/nomad-tools
 Description-Content-Type: text/markdown
```

### Comparing `nomad_tools-0.3.1/src/nomad_tools.egg-info/SOURCES.txt` & `nomad_tools-0.3.2/src/nomad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/tests/test_nomad_cp_complete.py` & `nomad_tools-0.3.2/tests/test_nomad_cp_complete.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/tests/test_taskexec_transfer_stats.py` & `nomad_tools-0.3.2/tests/test_taskexec_transfer_stats.py`

 * *Files identical despite different names*

### Comparing `nomad_tools-0.3.1/tests/testlib.py` & `nomad_tools-0.3.2/tests/testlib.py`

 * *Files identical despite different names*

