# Comparing `tmp/autotiling-1.9.1.tar.gz` & `tmp/autotiling-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotiling-1.9.1.tar", last modified: Tue Feb 27 22:22:40 2024, max compression
+gzip compressed data, was "autotiling-1.9.3.tar", last modified: Tue May 21 22:39:26 2024, max compression
```

## Comparing `autotiling-1.9.1.tar` & `autotiling-1.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:22:40.159488 autotiling-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-27 22:22:22.000000 autotiling-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-27 22:22:40.159488 autotiling-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-02-27 22:22:22.000000 autotiling-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:22:40.159488 autotiling-1.9.1/autotiling/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-27 22:22:22.000000 autotiling-1.9.1/autotiling/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-27 22:22:22.000000 autotiling-1.9.1/autotiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-02-27 22:22:22.000000 autotiling-1.9.1/autotiling/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 22:22:40.159488 autotiling-1.9.1/autotiling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-27 22:22:40.000000 autotiling-1.9.1/autotiling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-27 22:22:40.000000 autotiling-1.9.1/autotiling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 22:22:40.000000 autotiling-1.9.1/autotiling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-27 22:22:40.000000 autotiling-1.9.1/autotiling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-27 22:22:40.000000 autotiling-1.9.1/autotiling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 22:22:40.000000 autotiling-1.9.1/autotiling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-27 22:22:22.000000 autotiling-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-27 22:22:40.159488 autotiling-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-27 22:22:22.000000 autotiling-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:39:26.617585 autotiling-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 22:39:21.000000 autotiling-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-21 22:39:26.617585 autotiling-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-21 22:39:21.000000 autotiling-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:39:26.617585 autotiling-1.9.3/autotiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-21 22:39:21.000000 autotiling-1.9.3/autotiling/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-21 22:39:21.000000 autotiling-1.9.3/autotiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-21 22:39:21.000000 autotiling-1.9.3/autotiling/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:39:26.617585 autotiling-1.9.3/autotiling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-21 22:39:26.000000 autotiling-1.9.3/autotiling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-21 22:39:26.000000 autotiling-1.9.3/autotiling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:39:26.000000 autotiling-1.9.3/autotiling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 22:39:26.000000 autotiling-1.9.3/autotiling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 22:39:26.000000 autotiling-1.9.3/autotiling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 22:39:26.000000 autotiling-1.9.3/autotiling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 22:39:21.000000 autotiling-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-21 22:39:26.617585 autotiling-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 22:39:21.000000 autotiling-1.9.3/setup.py
```

### Comparing `autotiling-1.9.1/LICENSE` & `autotiling-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autotiling-1.9.1/PKG-INFO` & `autotiling-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotiling
-Version: 1.9.1
+Version: 1.9.3
 Summary: Automatically switch the horizontal/vertical window split orientation in sway and i3
 Home-page: https://github.com/nwg-piotr/autotiling
 Author: Piotr Miller
 Author-email: nwg.piotr@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Code, https://github.com/nwg-piotr/autotiling
 Project-URL: Issues, https://github.com/nwg-piotr/autotiling/issues
```

### Comparing `autotiling-1.9.1/README.md` & `autotiling-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `autotiling-1.9.1/autotiling/main.py` & `autotiling-1.9.3/autotiling/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,16 +123,16 @@
         elif debug:
             print("Debug: No focused container found or autotiling on the workspace turned off", file=sys.stderr)
 
     except Exception as e:
         print(f"Error: {e}", file=sys.stderr)
 
 
-def main():
-    parser = argparse.ArgumentParser()
+def get_parser():
+    parser = argparse.ArgumentParser(prog="autotiling", description="Script for sway and i3 to automatically switch the horizontal / vertical window split orientation")
 
     parser.add_argument("-d", "--debug", action="store_true",
                         help="print debug messages to stderr")
     parser.add_argument("-v", "--version", action="version",
                         version=f"%(prog)s {__version__}, Python {sys.version}",
                         help="display version information")
     parser.add_argument("-o", "--outputs", nargs="*", type=str, default=[],
@@ -162,15 +162,18 @@
     """
     Changing event subscription has already been the objective of several pull request. To avoid doing this again
     and again, let's allow to specify them in the `--events` argument.
     """
     parser.add_argument("-e", "--events", nargs="*", type=str, default=["WINDOW", "MODE"],
                         help="list of events to trigger switching split orientation; default: WINDOW MODE")
 
-    args = parser.parse_args()
+    return parser
+
+def main():
+    args = get_parser().parse_args()
 
     if args.debug:
         if args.outputs:
             print(f"autotiling is only active on outputs: {','.join(args.outputs)}")
         if args.workspaces:
             print(f"autotiling is only active on workspaces: {','.join(args.workspaces)}")
```

### Comparing `autotiling-1.9.1/autotiling.egg-info/PKG-INFO` & `autotiling-1.9.3/autotiling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotiling
-Version: 1.9.1
+Version: 1.9.3
 Summary: Automatically switch the horizontal/vertical window split orientation in sway and i3
 Home-page: https://github.com/nwg-piotr/autotiling
 Author: Piotr Miller
 Author-email: nwg.piotr@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Code, https://github.com/nwg-piotr/autotiling
 Project-URL: Issues, https://github.com/nwg-piotr/autotiling/issues
```

### Comparing `autotiling-1.9.1/setup.cfg` & `autotiling-1.9.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [metadata]
 name = autotiling
-version = 1.9.1
+version = 1.9.3
 author = Piotr Miller
 author_email = nwg.piotr@gmail.com
 description = Automatically switch the horizontal/vertical window split orientation in sway and i3
 url = https://github.com/nwg-piotr/autotiling
 project_urls = 
 	Code=https://github.com/nwg-piotr/autotiling
 	Issues=https://github.com/nwg-piotr/autotiling/issues
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPL-3.0-or-later
-license_file = LICENSE
+license_files = 
+	LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
```

