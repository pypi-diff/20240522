# Comparing `tmp/domaintools_api_v2-2.0.2.tar.gz` & `tmp/domaintools_api_v2-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domaintools_api_v2-2.0.2.tar", last modified: Fri May 17 14:56:38 2024, max compression
+gzip compressed data, was "domaintools_api_v2-2.0.3.tar", last modified: Wed May 22 13:24:31 2024, max compression
```

## Comparing `domaintools_api_v2-2.0.2.tar` & `domaintools_api_v2-2.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.670730 domaintools_api_v2-2.0.2/
--rw-r--r--   0 bluza      (502) staff       (20)     1078 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/LICENSE
--rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-17 14:56:38.670505 domaintools_api_v2-2.0.2/PKG-INFO
--rw-r--r--   0 bluza      (502) staff       (20)     7230 2024-03-04 18:03:36.000000 domaintools_api_v2-2.0.2/README.md
--rw-r--r--   0 bluza      (502) staff       (20)        5 2024-05-17 14:55:43.000000 domaintools_api_v2-2.0.2/VERSION
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.661265 domaintools_api_v2-2.0.2/domaintools/
--rw-r--r--   0 bluza      (502) staff       (20)      135 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     1181 2024-05-17 14:55:47.000000 domaintools_api_v2-2.0.2/domaintools/_version.py
--rw-r--r--   0 bluza      (502) staff       (20)    40580 2024-05-17 14:15:19.000000 domaintools_api_v2-2.0.2/domaintools/api.py
--rw-r--r--   0 bluza      (502) staff       (20)     8893 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools/base_results.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.664267 domaintools_api_v2-2.0.2/domaintools/cli/
--rw-r--r--   0 bluza      (502) staff       (20)      141 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     7717 2024-05-17 14:55:21.000000 domaintools_api_v2-2.0.2/domaintools/cli/api.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.666942 domaintools_api_v2-2.0.2/domaintools/cli/commands/
--rw-r--r--   0 bluza      (502) staff       (20)      133 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     2822 2024-05-17 14:30:51.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/accounts.py
--rw-r--r--   0 bluza      (502) staff       (20)    18505 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/detects.py
--rw-r--r--   0 bluza      (502) staff       (20)    23368 2024-04-29 16:18:47.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/domains.py
--rw-r--r--   0 bluza      (502) staff       (20)     6835 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/ips.py
--rw-r--r--   0 bluza      (502) staff       (20)     6452 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/iris.py
--rw-r--r--   0 bluza      (502) staff       (20)     3315 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/commands/phisheye.py
--rw-r--r--   0 bluza      (502) staff       (20)     1266 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/domaintools/cli/constants.py
--rw-r--r--   0 bluza      (502) staff       (20)      513 2024-05-17 14:34:04.000000 domaintools_api_v2-2.0.2/domaintools/cli/main.py
--rw-r--r--   0 bluza      (502) staff       (20)     6050 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.2/domaintools/cli/utils.py
--rw-r--r--   0 bluza      (502) staff       (20)      687 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools/exceptions.py
--rw-r--r--   0 bluza      (502) staff       (20)     3674 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools/results.py
--rw-r--r--   0 bluza      (502) staff       (20)     5619 2024-05-17 14:15:19.000000 domaintools_api_v2-2.0.2/domaintools/utils.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.669870 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/
--rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/PKG-INFO
--rw-r--r--   0 bluza      (502) staff       (20)      961 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/SOURCES.txt
--rw-r--r--   0 bluza      (502) staff       (20)        1 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/dependency_links.txt
--rw-r--r--   0 bluza      (502) staff       (20)       52 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/entry_points.txt
--rw-r--r--   0 bluza      (502) staff       (20)       37 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/requires.txt
--rw-r--r--   0 bluza      (502) staff       (20)       30 2024-05-17 14:56:38.000000 domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/top_level.txt
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.668049 domaintools_api_v2-2.0.2/domaintools_async/
--rw-r--r--   0 bluza      (502) staff       (20)     3015 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/domaintools_async/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     1453 2024-05-17 14:15:46.000000 domaintools_api_v2-2.0.2/pyproject.toml
--rw-r--r--   0 bluza      (502) staff       (20)      172 2024-05-17 14:56:38.671049 domaintools_api_v2-2.0.2/setup.cfg
--rwxr-xr-x   0 bluza      (502) staff       (20)     1541 2024-04-11 04:41:30.000000 domaintools_api_v2-2.0.2/setup.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-17 14:56:38.669078 domaintools_api_v2-2.0.2/tests/
--rw-r--r--   0 bluza      (502) staff       (20)    15279 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/tests/test_api.py
--rw-r--r--   0 bluza      (502) staff       (20)     1760 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/tests/test_async.py
--rw-r--r--   0 bluza      (502) staff       (20)     1045 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.2/tests/test_cli.py
--rw-r--r--   0 bluza      (502) staff       (20)     4055 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.2/tests/test_utils.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-22 13:24:31.446025 domaintools_api_v2-2.0.3/
+-rw-r--r--   0 bluza      (502) staff       (20)     1078 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.3/LICENSE
+-rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-22 13:24:31.445856 domaintools_api_v2-2.0.3/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)     7230 2024-03-04 18:03:36.000000 domaintools_api_v2-2.0.3/README.md
+-rw-r--r--   0 bluza      (502) staff       (20)        5 2024-05-22 13:21:31.000000 domaintools_api_v2-2.0.3/VERSION
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-22 13:24:31.437568 domaintools_api_v2-2.0.3/domaintools/
+-rw-r--r--   0 bluza      (502) staff       (20)      135 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/domaintools/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1181 2024-05-22 13:21:28.000000 domaintools_api_v2-2.0.3/domaintools/_version.py
+-rw-r--r--   0 bluza      (502) staff       (20)    40580 2024-05-17 14:15:19.000000 domaintools_api_v2-2.0.3/domaintools/api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     8893 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.3/domaintools/base_results.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-22 13:24:31.439497 domaintools_api_v2-2.0.3/domaintools/cli/
+-rw-r--r--   0 bluza      (502) staff       (20)      141 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/domaintools/cli/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     7684 2024-05-22 13:20:25.000000 domaintools_api_v2-2.0.3/domaintools/cli/api.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-22 13:24:31.442253 domaintools_api_v2-2.0.3/domaintools/cli/commands/
+-rw-r--r--   0 bluza      (502) staff       (20)      133 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/domaintools/cli/commands/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     2823 2024-05-17 15:07:34.000000 domaintools_api_v2-2.0.3/domaintools/cli/commands/accounts.py
+-rw-r--r--   0 bluza      (502) staff       (20)    18505 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/domaintools/cli/commands/detects.py
+-rw-r--r--   0 bluza      (502) staff       (20)    23368 2024-04-29 16:18:47.000000 domaintools_api_v2-2.0.3/domaintools/cli/commands/domains.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6835 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/domaintools/cli/commands/ips.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6452 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.3/domaintools/cli/commands/iris.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3315 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/domaintools/cli/commands/phisheye.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1266 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/domaintools/cli/constants.py
+-rw-r--r--   0 bluza      (502) staff       (20)      513 2024-05-17 14:34:04.000000 domaintools_api_v2-2.0.3/domaintools/cli/main.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6050 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.3/domaintools/cli/utils.py
+-rw-r--r--   0 bluza      (502) staff       (20)      687 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.3/domaintools/exceptions.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3674 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.3/domaintools/results.py
+-rw-r--r--   0 bluza      (502) staff       (20)     5619 2024-05-17 14:15:19.000000 domaintools_api_v2-2.0.3/domaintools/utils.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-22 13:24:31.445359 domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/
+-rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-22 13:24:31.000000 domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)      961 2024-05-22 13:24:31.000000 domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 bluza      (502) staff       (20)        1 2024-05-22 13:24:31.000000 domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       52 2024-05-22 13:24:31.000000 domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/entry_points.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       37 2024-05-22 13:24:31.000000 domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/requires.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       30 2024-05-22 13:24:31.000000 domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/top_level.txt
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-22 13:24:31.443583 domaintools_api_v2-2.0.3/domaintools_async/
+-rw-r--r--   0 bluza      (502) staff       (20)     3015 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.3/domaintools_async/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1453 2024-05-17 14:15:46.000000 domaintools_api_v2-2.0.3/pyproject.toml
+-rw-r--r--   0 bluza      (502) staff       (20)      172 2024-05-22 13:24:31.446287 domaintools_api_v2-2.0.3/setup.cfg
+-rwxr-xr-x   0 bluza      (502) staff       (20)     1541 2024-04-11 04:41:30.000000 domaintools_api_v2-2.0.3/setup.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-22 13:24:31.444941 domaintools_api_v2-2.0.3/tests/
+-rw-r--r--   0 bluza      (502) staff       (20)    15279 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.3/tests/test_api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1760 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.3/tests/test_async.py
+-rw-r--r--   0 bluza      (502) staff       (20)      997 2024-05-17 15:21:39.000000 domaintools_api_v2-2.0.3/tests/test_cli.py
+-rw-r--r--   0 bluza      (502) staff       (20)     4055 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.3/tests/test_utils.py
```

### Comparing `domaintools_api_v2-2.0.2/LICENSE` & `domaintools_api_v2-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/PKG-INFO` & `domaintools_api_v2-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domaintools_api_v2
-Version: 2.0.2
+Version: 2.0.3
 Summary: DomainTools Official Python API
 Author-email: DomainTools <integrations@domaintools.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 DomainTools
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.2 Summary:
+Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.3 Summary:
 DomainTools Official Python API Author-email: DomainTools
 domaintools.com> License: The MIT License (MIT) Copyright (c) 2016 DomainTools
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `domaintools_api_v2-2.0.2/README.md` & `domaintools_api_v2-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/_version.py` & `domaintools_api_v2-2.0.3/domaintools/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
-current = "2.0.2"
+current = "2.0.3"
```

### Comparing `domaintools_api_v2-2.0.2/domaintools/api.py` & `domaintools_api_v2-2.0.3/domaintools/api.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/base_results.py` & `domaintools_api_v2-2.0.3/domaintools/base_results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/api.py` & `domaintools_api_v2-2.0.3/domaintools/cli/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Optional, Dict, Tuple
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich import print
 
 from domaintools.api import API
 from domaintools.exceptions import ServiceException
 from domaintools.cli.utils import get_file_extension
-from domaintools.cli import constants
 
 
 class DTCLICommand:
     API_SUCCESS_STATUS = 200
     APP_PARTNER_NAME = "python_wrapper_cli_2.0.0"
 
     @staticmethod
@@ -190,15 +189,15 @@
 
                 output = cls._get_formatted_output(
                     cmd_name=name, response=response, out_format=response_format
                 )
 
                 if isinstance(out_file, _io.TextIOWrapper):
                     # use rich `print` command to prettify the ouput in sys.stdout
-                    print(output)
+                    typer.echo(output)
                 else:
                     # if it's a file then write
                     out_file.write(output if output.endswith("\n") else output + "\n")
                 time.sleep(0.5)
 
             name = typer.style(name, fg=typer.colors.CYAN, bold=True)
         except Exception as e:
```

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/commands/accounts.py` & `domaintools_api_v2-2.0.3/domaintools/cli/commands/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,11 +79,12 @@
     ),
     no_verify_ssl: bool = typer.Option(
         False,
         "--no-verify-ssl",
         help="Skip verification of SSL certificate when making HTTPs API calls",
     ),
 ):
+
     DTCLICommand.run(name=c.AVAILABLE_API_CALLS, params=ctx.params)
 
 
 __all__ = ["account_information", "available_api_calls"]
```

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/commands/detects.py` & `domaintools_api_v2-2.0.3/domaintools/cli/commands/detects.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/commands/domains.py` & `domaintools_api_v2-2.0.3/domaintools/cli/commands/domains.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/commands/ips.py` & `domaintools_api_v2-2.0.3/domaintools/cli/commands/ips.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/commands/iris.py` & `domaintools_api_v2-2.0.3/domaintools/cli/commands/iris.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/commands/phisheye.py` & `domaintools_api_v2-2.0.3/domaintools/cli/commands/phisheye.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/constants.py` & `domaintools_api_v2-2.0.3/domaintools/cli/constants.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/main.py` & `domaintools_api_v2-2.0.3/domaintools/cli/main.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/cli/utils.py` & `domaintools_api_v2-2.0.3/domaintools/cli/utils.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/exceptions.py` & `domaintools_api_v2-2.0.3/domaintools/exceptions.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/results.py` & `domaintools_api_v2-2.0.3/domaintools/results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools/utils.py` & `domaintools_api_v2-2.0.3/domaintools/utils.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/PKG-INFO` & `domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domaintools_api_v2
-Version: 2.0.2
+Version: 2.0.3
 Summary: DomainTools Official Python API
 Author-email: DomainTools <integrations@domaintools.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 DomainTools
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.2 Summary:
+Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.3 Summary:
 DomainTools Official Python API Author-email: DomainTools
 domaintools.com> License: The MIT License (MIT) Copyright (c) 2016 DomainTools
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `domaintools_api_v2-2.0.2/domaintools_api_v2.egg-info/SOURCES.txt` & `domaintools_api_v2-2.0.3/domaintools_api_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/domaintools_async/__init__.py` & `domaintools_api_v2-2.0.3/domaintools_async/__init__.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/pyproject.toml` & `domaintools_api_v2-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/setup.py` & `domaintools_api_v2-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/tests/test_api.py` & `domaintools_api_v2-2.0.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/tests/test_async.py` & `domaintools_api_v2-2.0.3/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.2/tests/test_cli.py` & `domaintools_api_v2-2.0.3/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 import os
 
 from typer.testing import CliRunner
 
 from domaintools.cli import dt_cli
 from domaintools._version import current
 
-from tests.settings import vcr
-
 runner = CliRunner()
 
 
 def test_match_cli_version():
     result = runner.invoke(dt_cli, ["--version"])
 
     expected_res = f"DomainTools CLI API Client {current}"
     assert expected_res == result.stdout.strip()
 
 
 def test_valid_command():
     user = os.environ.get("TEST_USER", "test")
     key = os.environ.get("TEST_KEY", "key")
     result = runner.invoke(dt_cli, ["account_information", "--help"])
-    assert "About to execute command: `account_information`" in result.stdout
+    assert "Usage: main account_information" in result.stdout
 
 
 def test_invalid_command():
     result = runner.invoke(dt_cli, ["test_invalid_command"])
     assert "No such command 'test_invalid_command'." in result.stdout
```

### Comparing `domaintools_api_v2-2.0.2/tests/test_utils.py` & `domaintools_api_v2-2.0.3/tests/test_utils.py`

 * *Files identical despite different names*

