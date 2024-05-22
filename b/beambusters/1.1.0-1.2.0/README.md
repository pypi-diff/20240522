# Comparing `tmp/beambusters-1.1.0.tar.gz` & `tmp/beambusters-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.1.0.tar", max compression
+gzip compressed data, was "beambusters-1.2.0.tar", max compression
```

## Comparing `beambusters-1.1.0.tar` & `beambusters-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-22 12:05:01.019777 beambusters-1.1.0/LICENSE
--rw-r--r--   0        0        0      630 2024-05-22 12:05:01.019777 beambusters-1.1.0/README.md
--rwxr-xr-x   0        0        0        0 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/__init__.py
--rw-r--r--   0        0        0    11833 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/main.py
--rwxr-xr-x   0        0        0     3170 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/settings.py
--rwxr-xr-x   0        0        0      143 2024-05-22 12:05:01.019777 beambusters-1.1.0/beambusters/utils.py
--rw-r--r--   0        0        0     2026 2024-05-22 12:05:09.019782 beambusters-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 15:54:42.031692 beambusters-1.2.0/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-22 15:54:42.031692 beambusters-1.2.0/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/__init__.py
+-rw-r--r--   0        0        0    11827 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/main.py
+-rwxr-xr-x   0        0        0     3170 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/settings.py
+-rwxr-xr-x   0        0        0      143 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/utils.py
+-rw-r--r--   0        0        0     2026 2024-05-22 15:54:51.699699 beambusters-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.2.0/PKG-INFO
```

### Comparing `beambusters-1.1.0/LICENSE` & `beambusters-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.1.0/README.md` & `beambusters-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.1.0/beambusters/main.py` & `beambusters-1.2.0/beambusters/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     BeambustersParam = settings.parse(config)
     files = open(input, "r")
     paths = files.readlines()
     files.close()
 
     if len(paths[0][:-1].split(" //")) == 1:
         # Not listed events. TODO test if CrystFEL not loaded sucessfully.
-        list_name = sys.argv[1]
+        list_name = input
         events_list_file = (
             f"{list_name.split('.')[0]}_events.lst{list_name.split('.')[-1][-2:]}"
         )
         command = f"source /etc/profile.d/modules.sh; module load maxwell crystfel/0.11.0; list_events -i {list_name} -o {events_list_file} -g {config['geometry_file']}"
         sub.call(command, shell=True)
         files = open(events_list_file, "r")
         paths = files.readlines()
```

### Comparing `beambusters-1.1.0/beambusters/settings.py` & `beambusters-1.2.0/beambusters/settings.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.1.0/pyproject.toml` & `beambusters-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.1.0"
+version = "1.2.0"
 description = ""
 authors = ["Ana Rodrigues <anananacr@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 beambusters = "beambusters.main:app"
```

### Comparing `beambusters-1.1.0/PKG-INFO` & `beambusters-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: Ana Rodrigues
 Author-email: anananacr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

