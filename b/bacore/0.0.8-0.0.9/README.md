# Comparing `tmp/bacore-0.0.8.tar.gz` & `tmp/bacore-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacore-0.0.8.tar", last modified: Tue Jan 16 12:13:09 2024, max compression
+gzip compressed data, was "bacore-0.0.9.tar", last modified: Wed Jan 24 12:31:03 2024, max compression
```

## Comparing `bacore-0.0.8.tar` & `bacore-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.010692 bacore-0.0.8/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     3120 2024-01-09 09:42:50.000000 bacore-0.0.8/.gitignore
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1066 2023-12-15 17:36:35.000000 bacore-0.0.8/LICENSE
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     4193 2024-01-16 12:13:09.010192 bacore-0.0.8/PKG-INFO
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      357 2024-01-09 10:51:29.000000 bacore-0.0.8/README.md
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.000490 bacore-0.0.8/docs/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      197 2024-01-01 12:45:47.000000 bacore-0.0.8/docs/cli.md
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1164 2024-01-09 10:51:29.000000 bacore-0.0.8/docs/index.md
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1464 2023-12-26 06:00:54.000000 bacore-0.0.8/mkdocs.yml
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     2158 2024-01-16 12:10:35.000000 bacore-0.0.8/pyproject.toml
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      106 2024-01-06 16:28:27.000000 bacore-0.0.8/pytest.ini
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       38 2024-01-16 12:13:09.010815 bacore-0.0.8/setup.cfg
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:08.995938 bacore-0.0.8/src/
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.000914 bacore-0.0.8/src/bacore/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      146 2023-12-26 06:00:54.000000 bacore-0.0.8/src/bacore/__init__.py
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.003240 bacore-0.0.8/src/bacore/cli/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       57 2024-01-09 17:46:56.000000 bacore-0.0.8/src/bacore/cli/__init__.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      992 2024-01-15 06:50:55.000000 bacore-0.0.8/src/bacore/cli/create.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      580 2024-01-16 11:59:02.000000 bacore-0.0.8/src/bacore/cli/main.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1100 2024-01-15 06:50:55.000000 bacore-0.0.8/src/bacore/cli/serve.py
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.004462 bacore-0.0.8/src/bacore/domain/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2023-12-04 12:53:07.000000 bacore-0.0.8/src/bacore/domain/__init__.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1406 2024-01-15 20:37:37.000000 bacore-0.0.8/src/bacore/domain/config.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      498 2024-01-06 12:04:23.000000 bacore-0.0.8/src/bacore/domain/errors.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      736 2024-01-15 20:59:45.000000 bacore-0.0.8/src/bacore/domain/files.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      440 2024-01-15 21:33:03.000000 bacore-0.0.8/src/bacore/domain/system.py
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.005288 bacore-0.0.8/src/bacore/interactors/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2023-12-04 12:53:16.000000 bacore-0.0.8/src/bacore/interactors/__init__.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      666 2024-01-15 22:18:44.000000 bacore-0.0.8/src/bacore/interactors/retrieve.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      342 2024-01-15 21:13:52.000000 bacore-0.0.8/src/bacore/interactors/verify.py
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.006021 bacore-0.0.8/src/bacore/interfaces/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       35 2024-01-09 17:46:56.000000 bacore-0.0.8/src/bacore/interfaces/__init__.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      814 2024-01-16 12:02:09.000000 bacore-0.0.8/src/bacore/interfaces/api_fastapi.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1362 2024-01-16 11:59:58.000000 bacore-0.0.8/src/bacore/interfaces/cli_typer.py
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.007566 bacore-0.0.8/src/bacore.egg-info/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     4193 2024-01-16 12:13:08.000000 bacore-0.0.8/src/bacore.egg-info/PKG-INFO
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      910 2024-01-16 12:13:08.000000 bacore-0.0.8/src/bacore.egg-info/SOURCES.txt
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        1 2024-01-16 12:13:08.000000 bacore-0.0.8/src/bacore.egg-info/dependency_links.txt
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       47 2024-01-16 12:13:08.000000 bacore-0.0.8/src/bacore.egg-info/entry_points.txt
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      720 2024-01-16 12:13:08.000000 bacore-0.0.8/src/bacore.egg-info/requires.txt
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        7 2024-01-16 12:13:08.000000 bacore-0.0.8/src/bacore.egg-info/top_level.txt
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.006239 bacore-0.0.8/tests/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      432 2024-01-15 14:02:49.000000 bacore-0.0.8/tests/conftest.py
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.006683 bacore-0.0.8/tests/domain/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      921 2024-01-15 20:52:12.000000 bacore-0.0.8/tests/domain/test_config.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      738 2024-01-15 06:50:55.000000 bacore-0.0.8/tests/domain/test_files.py
-drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-16 12:13:09.007202 bacore-0.0.8/tests/interactors/
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      543 2024-01-15 20:29:38.000000 bacore-0.0.8/tests/interactors/test_retrieve.py
--rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      749 2024-01-15 21:44:01.000000 bacore-0.0.8/tests/interactors/test_verify.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.438454 bacore-0.0.9/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     3120 2024-01-09 09:42:50.000000 bacore-0.0.9/.gitignore
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1066 2023-12-15 17:36:35.000000 bacore-0.0.9/LICENSE
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     4193 2024-01-24 12:31:03.438044 bacore-0.0.9/PKG-INFO
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      357 2024-01-09 10:51:29.000000 bacore-0.0.9/README.md
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.427677 bacore-0.0.9/docs/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      197 2024-01-01 12:45:47.000000 bacore-0.0.9/docs/cli.md
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1164 2024-01-09 10:51:29.000000 bacore-0.0.9/docs/index.md
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1464 2023-12-26 06:00:54.000000 bacore-0.0.9/mkdocs.yml
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     2158 2024-01-24 12:30:47.000000 bacore-0.0.9/pyproject.toml
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      143 2024-01-24 11:30:55.000000 bacore-0.0.9/pytest.ini
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       38 2024-01-24 12:31:03.438525 bacore-0.0.9/setup.cfg
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.422654 bacore-0.0.9/src/
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.427989 bacore-0.0.9/src/bacore/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      146 2023-12-26 06:00:54.000000 bacore-0.0.9/src/bacore/__init__.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.430640 bacore-0.0.9/src/bacore/cli/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       57 2024-01-09 17:46:56.000000 bacore-0.0.9/src/bacore/cli/__init__.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1000 2024-01-23 11:47:01.000000 bacore-0.0.9/src/bacore/cli/create.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      580 2024-01-16 11:59:02.000000 bacore-0.0.9/src/bacore/cli/main.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1108 2024-01-23 11:47:01.000000 bacore-0.0.9/src/bacore/cli/serve.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.431810 bacore-0.0.9/src/bacore/domain/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2023-12-04 12:53:07.000000 bacore-0.0.9/src/bacore/domain/__init__.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1404 2024-01-23 11:47:01.000000 bacore-0.0.9/src/bacore/domain/config.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      498 2024-01-06 12:04:23.000000 bacore-0.0.9/src/bacore/domain/errors.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      736 2024-01-15 20:59:45.000000 bacore-0.0.9/src/bacore/domain/files.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      440 2024-01-15 21:33:03.000000 bacore-0.0.9/src/bacore/domain/system.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.432451 bacore-0.0.9/src/bacore/interactors/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2023-12-04 12:53:16.000000 bacore-0.0.9/src/bacore/interactors/__init__.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      666 2024-01-24 11:34:58.000000 bacore-0.0.9/src/bacore/interactors/retrieve.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      342 2024-01-15 21:13:52.000000 bacore-0.0.9/src/bacore/interactors/verify.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.433412 bacore-0.0.9/src/bacore/interfaces/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       35 2024-01-09 17:46:56.000000 bacore-0.0.9/src/bacore/interfaces/__init__.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1209 2024-01-24 11:57:59.000000 bacore-0.0.9/src/bacore/interfaces/api_fastapi.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     1872 2024-01-24 11:36:28.000000 bacore-0.0.9/src/bacore/interfaces/cli_typer.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.435378 bacore-0.0.9/src/bacore.egg-info/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)     4193 2024-01-24 12:31:03.000000 bacore-0.0.9/src/bacore.egg-info/PKG-INFO
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      945 2024-01-24 12:31:03.000000 bacore-0.0.9/src/bacore.egg-info/SOURCES.txt
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        1 2024-01-24 12:31:03.000000 bacore-0.0.9/src/bacore.egg-info/dependency_links.txt
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)       47 2024-01-24 12:31:03.000000 bacore-0.0.9/src/bacore.egg-info/entry_points.txt
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      720 2024-01-24 12:31:03.000000 bacore-0.0.9/src/bacore.egg-info/requires.txt
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        7 2024-01-24 12:31:03.000000 bacore-0.0.9/src/bacore.egg-info/top_level.txt
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.433623 bacore-0.0.9/tests/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      432 2024-01-15 14:02:49.000000 bacore-0.0.9/tests/conftest.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.434137 bacore-0.0.9/tests/domain/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      937 2024-01-24 12:17:30.000000 bacore-0.0.9/tests/domain/test_config.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      738 2024-01-15 06:50:55.000000 bacore-0.0.9/tests/domain/test_files.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.434617 bacore-0.0.9/tests/interactors/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      543 2024-01-24 11:24:33.000000 bacore-0.0.9/tests/interactors/test_retrieve.py
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      749 2024-01-15 21:44:01.000000 bacore-0.0.9/tests/interactors/test_verify.py
+drwxr-xr-x   0 kgronber (1810213900) DOM01\Domain Users (1841270448)        0 2024-01-24 12:31:03.434848 bacore-0.0.9/tests/interfaces/
+-rw-r--r--   0 kgronber (1810213900) DOM01\Domain Users (1841270448)      464 2024-01-24 12:20:52.000000 bacore-0.0.9/tests/interfaces/test_cli_typer.py
```

### Comparing `bacore-0.0.8/.gitignore` & `bacore-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/LICENSE` & `bacore-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/PKG-INFO` & `bacore-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacore
-Version: 0.0.8
+Version: 0.0.9
 Summary: BACore is a framework for business analysis and test automation.
 Author-email: Kristian Grönberg <kristian@gronberg.org>, Jacob Dahlberg <dahlberg.jacob@gmail.com>, Jonatan Söderström <jonatan.m.soderstrom@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 bacoredev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bacore-0.0.8/docs/index.md` & `bacore-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/mkdocs.yml` & `bacore-0.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/pyproject.toml` & `bacore-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=60.2.0', 'setuptools-scm', "mypy"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'bacore'
-version = "0.0.8"
+version = "0.0.9"
 description = "BACore is a framework for business analysis and test automation."
 readme = "README.md"
 authors = [
     { name = "Kristian Grönberg", email = "kristian@gronberg.org" },
     { name = "Jacob Dahlberg", email = "dahlberg.jacob@gmail.com"},
     { name = "Jonatan Söderström", email = "jonatan.m.soderstrom@gmail.com"}]
 license = { file = "LICENSE" }
```

### Comparing `bacore-0.0.8/src/bacore/cli/create.py` & `bacore-0.0.9/src/bacore/cli/create.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Create CLI module."""
 import subprocess as sup
-from bacore.domain.config import Project
+from bacore.domain.config import ProjectInfo
 from bacore.domain.errors import PydValErrInfo
 from bacore.interfaces import cli_typer
 from pydantic import ValidationError
 from rich import print
 from typer import Argument, Exit, Typer, prompt
 from typing import Annotated
 
@@ -16,14 +16,14 @@
     """Create new project ([blue]with hatch[/])."""
     cli_typer.verify_programs_installed(['hatch'])
 
     if name == '':
         name = prompt("Enter project name")
 
     try:
-        new_project = Project(name=name)
+        new_project = ProjectInfo(name=name)
     except ValidationError as e:
         print(f'[red]{PydValErrInfo.error_msg(e)}[/red] Input was: "{PydValErrInfo.input(e)}"')
         raise Exit()
 
     print(f'Creating new project "{new_project.name}"[white]...[/]')
     sup.run(f'hatch new {new_project.name}', shell=True)
```

### Comparing `bacore-0.0.8/src/bacore/cli/main.py` & `bacore-0.0.9/src/bacore/cli/main.py`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/src/bacore/cli/serve.py` & `bacore-0.0.9/src/bacore/cli/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Serve CLI module."""
 import subprocess as sup
-from bacore.domain.config import Project
+from bacore.domain.config import ProjectInfo
 from bacore.domain.errors import PydValErrInfo
 from bacore.interfaces import cli_typer
 from pydantic import ValidationError
 from rich import print
 from typer import Argument, Exit, Option, Typer, prompt
 from typing import Annotated
 
@@ -17,14 +17,14 @@
     """Serve documentation with MkDocs for a project."""
     cli_typer.verify_programs_installed(['mkdocs'])
 
     if project == '':
         project = prompt("Enter project name")
 
     try:
-        project = Project(name=project)
+        project = ProjectInfo(name=project)
     except ValidationError as e:
         print(f'[red]{PydValErrInfo.error_msg(e)}[/red] Input was: "{PydValErrInfo.input(e)}"')
         raise Exit()
 
     print(f'Serving documentation for project "{project.name}"[white]...[/]')
     sup.run(f"mkdocs serve -a 127.0.0.1:{port} &", shell=True)
```

### Comparing `bacore-0.0.8/src/bacore/domain/config.py` & `bacore-0.0.9/src/bacore/domain/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         """Validate that the username does not contain spaces."""
         if " " in v:
             raise ValueError("No spaces allowed in username.")
         return v
 
 
 @dataclass
-class Project:
-    """Project configurations."""
+class ProjectInfo:
+    """Project information."""
 
     name: str
     version: Optional[str] = None
     description: Optional[str] = None
 
     @field_validator("name")
     @classmethod
@@ -35,15 +35,15 @@
         if " " in v:
             raise ValueError("No spaces allowed in project name.")
         return v
 
 
 @dataclass
 class SystemInfo:
-    """System configurations."""
+    """System information."""
 
     os: str
 
     @field_validator("os")
     @classmethod
     def os_must_be_supported(cls, v: str) -> str:
         """Validate that the operating system is supported."""
```

### Comparing `bacore-0.0.8/src/bacore/domain/files.py` & `bacore-0.0.9/src/bacore/domain/files.py`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/src/bacore/interactors/retrieve.py` & `bacore-0.0.9/src/bacore/interactors/retrieve.py`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/src/bacore/interfaces/api_fastapi.py` & `bacore-0.0.9/src/bacore/interfaces/api_fastapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Web API with FastAPI."""
-from bacore.domain import files
+from bacore.domain import config, files
 from bacore.interactors import retrieve
 from pathlib import Path
+from typing import Optional
 
 
 class ProjectInfo:
-    """Project information."""
+    """ProjectInfo information."""
 
     def __init__(self, pyproject_file: Path):
         """Initialize."""
         self._pyproject_file_toml_object = files.TOML(path=pyproject_file)
-        self._project_info = retrieve.file_as_dict(file=self._pyproject_file_toml_object)
+        self._project_info_dict = retrieve.file_as_dict(file=self._pyproject_file_toml_object)
+        self._project_info = config.ProjectInfo(name=self._project_info_dict["project"]["name"],
+                                                version=self._project_info_dict["project"]["version"],
+                                                description=self._project_info_dict["project"]["description"]
+                                                )
 
     @property
     def name(self) -> str:
-        """Project name."""
-        return self._project_info["project"]["name"]
+        """ProjectInfo name."""
+        return self._project_info.name
 
     @property
-    def version(self) -> str:
-        """Project version."""
-        return self._project_info["project"]["version"]
+    def version(self) -> Optional[str]:
+        """ProjectInfo version."""
+        return self._project_info.version
 
     @property
-    def description(self) -> str:
-        """Project description."""
-        return self._project_info["project"]["description"]
+    def description(self) -> Optional[str]:
+        """ProjectInfo description."""
+        return self._project_info.description
```

### Comparing `bacore-0.0.8/src/bacore/interfaces/cli_typer.py` & `bacore-0.0.9/src/bacore/interfaces/cli_typer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 """CLI created with Typer."""
-from bacore.domain import files, system
+from bacore.domain import config, files, system
 from bacore.interactors import retrieve, verify
 from rich import print
 from pathlib import Path
 from typer import Exit
+from typing import Optional
 
 
 class ProjectInfo:
-    """Project information."""
+    """ProjectInfo information."""
 
     def __init__(self, pyproject_file: Path):
         """Initialize."""
         self._pyproject_file_toml_object = files.TOML(path=pyproject_file)
-        self._project_info = retrieve.file_as_dict(file=self._pyproject_file_toml_object)
+        self._project_info_dict = retrieve.file_as_dict(file=self._pyproject_file_toml_object)
+        self._project_info = config.ProjectInfo(name=self._project_info_dict["project"]["name"],
+                                                version=self._project_info_dict["project"]["version"],
+                                                description=self._project_info_dict["project"]["description"]
+                                                )
 
     @property
     def name(self) -> str:
-        """Project name."""
-        return self._project_info["project"]["name"]
+        """ProjectInfo name."""
+        return self._project_info.name
 
     @property
-    def version(self) -> str:
-        """Project version."""
-        return self._project_info["project"]["version"]
+    def version(self) -> Optional[str]:
+        """ProjectInfo version."""
+        return self._project_info.version
 
     @property
-    def description(self) -> str:
-        """Project description."""
-        return self._project_info["project"]["description"]
+    def description(self) -> Optional[str]:
+        """ProjectInfo description."""
+        return self._project_info.description
 
 
 def verify_programs_installed(list_of_programs: list[system.CommandLineProgram]):
-    """Check if a list of command line programs are installed."""
+    """Check if a list of command line programs are installed.
+
+    TODO: This function does not follow the overall design of the project. -> Move to an interactor module.
+
+    """
     programs_not_installed = 0
 
     for program in list_of_programs:
         if verify.command_on_path(program) is False:
             programs_not_installed += 1
             print(f'{program} is [red]not installed[/]. Install with: [blue]pip install bacore\\[cli\\][/]')
```

### Comparing `bacore-0.0.8/src/bacore.egg-info/PKG-INFO` & `bacore-0.0.9/src/bacore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacore
-Version: 0.0.8
+Version: 0.0.9
 Summary: BACore is a framework for business analysis and test automation.
 Author-email: Kristian Grönberg <kristian@gronberg.org>, Jacob Dahlberg <dahlberg.jacob@gmail.com>, Jonatan Söderström <jonatan.m.soderstrom@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 bacoredev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bacore-0.0.8/src/bacore.egg-info/SOURCES.txt` & `bacore-0.0.9/src/bacore.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 src/bacore/interfaces/__init__.py
 src/bacore/interfaces/api_fastapi.py
 src/bacore/interfaces/cli_typer.py
 tests/conftest.py
 tests/domain/test_config.py
 tests/domain/test_files.py
 tests/interactors/test_retrieve.py
-tests/interactors/test_verify.py
+tests/interactors/test_verify.py
+tests/interfaces/test_cli_typer.py
```

### Comparing `bacore-0.0.8/src/bacore.egg-info/requires.txt` & `bacore-0.0.9/src/bacore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/tests/domain/test_config.py` & `bacore-0.0.9/tests/domain/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Tests for domain.config module."""
 import pytest
 from bacore.domain import config
 
 pytestmark = pytest.mark.domain
 
 
-class TestProject:
-    """Tests for Project entity."""
+class TestProjectInfo:
+    """Tests for ProjectInfo entity."""
 
     def test_name(self):
         """Test name."""
-        p = config.Project(name="bacore")
+        p = config.ProjectInfo(name="bacore")
         assert p.name == "bacore"
 
     def test_name_must_not_contain_spaces(self):
         """Test name_must_not_contain_spaces."""
         with pytest.raises(ValueError):
-            config.Project(name="ba core")
+            config.ProjectInfo(name="ba core")
 
 
 class TestSystemInfo:
     """Test for SystemInfo."""
 
     def test_os(self):
         """Test os. (Darwin is macOS.)"""
```

### Comparing `bacore-0.0.8/tests/domain/test_files.py` & `bacore-0.0.9/tests/domain/test_files.py`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/tests/interactors/test_retrieve.py` & `bacore-0.0.9/tests/interactors/test_retrieve.py`

 * *Files identical despite different names*

### Comparing `bacore-0.0.8/tests/interactors/test_verify.py` & `bacore-0.0.9/tests/interactors/test_verify.py`

 * *Files identical despite different names*

