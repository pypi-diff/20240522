# Comparing `tmp/flort-0.1.6.3.tar.gz` & `tmp/flort-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flort-0.1.6.3.tar", last modified: Tue May 14 18:05:07 2024, max compression
+gzip compressed data, was "flort-0.1.7.1.tar", last modified: Wed May 22 13:10:12 2024, max compression
```

## Comparing `flort-0.1.6.3.tar` & `flort-0.1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 18:05:07.716765 flort-0.1.6.3/
--rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.6.3/LICENSE
--rw-r--r--   0 nd        (1000) nd        (1000)     1743 2024-05-14 18:05:07.716765 flort-0.1.6.3/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)     1264 2024-04-04 14:43:55.000000 flort-0.1.6.3/README.md
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 18:05:07.715765 flort-0.1.6.3/flort/
--rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.6.3/flort/__init__.py
--rw-r--r--   0 nd        (1000) nd        (1000)       61 2024-05-14 17:13:43.000000 flort-0.1.6.3/flort/__main__.py
--rw-r--r--   0 nd        (1000) nd        (1000)     6352 2024-05-14 18:04:40.000000 flort-0.1.6.3/flort/cli.py
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 18:05:07.716765 flort-0.1.6.3/flort.egg-info/
--rw-r--r--   0 nd        (1000) nd        (1000)     1743 2024-05-14 18:05:07.000000 flort-0.1.6.3/flort.egg-info/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)      287 2024-05-14 18:05:07.000000 flort-0.1.6.3/flort.egg-info/SOURCES.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-05-14 18:05:07.000000 flort-0.1.6.3/flort.egg-info/dependency_links.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-05-14 18:05:07.000000 flort-0.1.6.3/flort.egg-info/entry_points.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        9 2024-05-14 18:05:07.000000 flort-0.1.6.3/flort.egg-info/requires.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       12 2024-05-14 18:05:07.000000 flort-0.1.6.3/flort.egg-info/top_level.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-05-14 18:05:07.716765 flort-0.1.6.3/setup.cfg
--rw-r--r--   0 nd        (1000) nd        (1000)      803 2024-05-14 18:05:05.000000 flort-0.1.6.3/setup.py
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 18:05:07.716765 flort-0.1.6.3/tests/
--rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-05-14 17:20:58.000000 flort-0.1.6.3/tests/__init__.py
--rw-r--r--   0 nd        (1000) nd        (1000)     4272 2024-05-14 18:01:17.000000 flort-0.1.6.3/tests/test_cli.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-22 13:10:12.475284 flort-0.1.7.1/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.7.1/LICENSE
+-rw-r--r--   0 nd        (1000) nd        (1000)     3114 2024-05-22 13:10:12.475284 flort-0.1.7.1/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)     2658 2024-05-14 18:10:36.000000 flort-0.1.7.1/README.md
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-22 13:10:12.473284 flort-0.1.7.1/flort/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.7.1/flort/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)       61 2024-05-14 17:13:43.000000 flort-0.1.7.1/flort/__main__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     6457 2024-05-22 13:10:01.000000 flort-0.1.7.1/flort/cli.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-22 13:10:12.474284 flort-0.1.7.1/flort.egg-info/
+-rw-r--r--   0 nd        (1000) nd        (1000)     3114 2024-05-22 13:10:12.000000 flort-0.1.7.1/flort.egg-info/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)      287 2024-05-22 13:10:12.000000 flort-0.1.7.1/flort.egg-info/SOURCES.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-05-22 13:10:12.000000 flort-0.1.7.1/flort.egg-info/dependency_links.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-05-22 13:10:12.000000 flort-0.1.7.1/flort.egg-info/entry_points.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        9 2024-05-22 13:10:12.000000 flort-0.1.7.1/flort.egg-info/requires.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       12 2024-05-22 13:10:12.000000 flort-0.1.7.1/flort.egg-info/top_level.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-05-22 13:10:12.475284 flort-0.1.7.1/setup.cfg
+-rw-r--r--   0 nd        (1000) nd        (1000)      803 2024-05-22 13:08:22.000000 flort-0.1.7.1/setup.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-22 13:10:12.474284 flort-0.1.7.1/tests/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-05-14 17:20:58.000000 flort-0.1.7.1/tests/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     4272 2024-05-14 18:01:17.000000 flort-0.1.7.1/tests/test_cli.py
```

### Comparing `flort-0.1.6.3/LICENSE` & `flort-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flort-0.1.6.3/flort/cli.py` & `flort-0.1.7.1/flort/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,16 +105,17 @@
     logging.info(f"Directories being processed: {', '.join(directories)}")
     logging.info(f"File extensions being processed: {', '.join(extensions)}")
     logging.info(f"Including all files: {include_all}")
     logging.info(f"Including hidden files: {include_hidden}")
 
 def main():
     """Main function to parse arguments and execute operations."""
-    parser = argparse.ArgumentParser(description="flort: create a single file of all given extensions, recursivly for all dirictories given. Ignores binary files.", prog='flort')
+    parser = argparse.ArgumentParser(description="flort: create a single file of all given extensions, recursivly for all dirictories given. Ignores binary files.", prog='flort', add_help=False)
     parser.add_argument('directories', metavar='DIRECTORY', type=str, nargs='+', help='Directories to list files from.')
+    parser.add_argument('--help', action='help', help='show this help message and exit')
     parser.add_argument('--output', type=str, default="stdio", help='Output file path. Defaults to stdout if not specified.')
     parser.add_argument('--no-tree', action='store_true', help='Do not print the tree at the beginning.')
     parser.add_argument('--all', action='store_true', help='Include all files regardless of extensions.')
     parser.add_argument('--hidden', action='store_true', help='Include hidden files.')
     args, unknown_args = parser.parse_known_args()
 
     # Treat unknown args as extensions that start with '--'
```

### Comparing `flort-0.1.6.3/setup.py` & `flort-0.1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flort',
-    version='0.1.6.3',
+    version='0.1.7.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'flort = flort.__main__:main'
         ]
     },
     install_requires=[
```

### Comparing `flort-0.1.6.3/tests/test_cli.py` & `flort-0.1.7.1/tests/test_cli.py`

 * *Files identical despite different names*

