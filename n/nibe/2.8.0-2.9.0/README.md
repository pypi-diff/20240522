# Comparing `tmp/nibe-2.8.0.tar.gz` & `tmp/nibe-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibe-2.8.0.tar", last modified: Mon Feb  5 08:41:53 2024, max compression
+gzip compressed data, was "nibe-2.9.0.tar", last modified: Tue Feb 27 07:41:22 2024, max compression
```

## Comparing `nibe-2.8.0.tar` & `nibe-2.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:53.989760 nibe-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-05 08:41:44.000000 nibe-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43802 2024-02-05 08:41:53.989760 nibe-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-02-05 08:41:44.000000 nibe-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:53.981760 nibe-2.8.0/nibe/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/coil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/coil_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:53.981760 nibe-2.8.0/nibe/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/connection/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/connection/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/connection/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25848 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/connection/nibegw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:53.981760 nibe-2.8.0/nibe/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/console_scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/console_scripts/convert_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:53.989760 nibe-2.8.0/nibe/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)   349701 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/f1145_f1245.json
--rw-r--r--   0 runner    (1001) docker     (127)   235705 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/f1155_f1255.json
--rw-r--r--   0 runner    (1001) docker     (127)   363545 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/f1345.json
--rw-r--r--   0 runner    (1001) docker     (127)   371005 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/f1355.json
--rw-r--r--   0 runner    (1001) docker     (127)   112391 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/f370_f470.json
--rw-r--r--   0 runner    (1001) docker     (127)   133339 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/f730.json
--rw-r--r--   0 runner    (1001) docker     (127)   149841 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/f750.json
--rw-r--r--   0 runner    (1001) docker     (127)   257358 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/s1155_s1255.json
--rw-r--r--   0 runner    (1001) docker     (127)   152644 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/s2125.json
--rw-r--r--   0 runner    (1001) docker     (127)   167771 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/s320_s325.json
--rw-r--r--   0 runner    (1001) docker     (127)   184019 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/s735.json
--rw-r--r--   0 runner    (1001) docker     (127)    81905 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/smo20.json
--rw-r--r--   0 runner    (1001) docker     (127)   302335 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/smo40.json
--rw-r--r--   0 runner    (1001) docker     (127)   243617 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/smos40.json
--rw-r--r--   0 runner    (1001) docker     (127)   210922 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/vvm225_vvm320_vvm325.json
--rw-r--r--   0 runner    (1001) docker     (127)   206182 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/data/vvm310_vvm500.json
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/event_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/heatpump.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:44.000000 nibe-2.8.0/nibe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:53.989760 nibe-2.8.0/nibe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43802 2024-02-05 08:41:53.000000 nibe-2.8.0/nibe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-05 08:41:53.000000 nibe-2.8.0/nibe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 08:41:53.000000 nibe-2.8.0/nibe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-05 08:41:53.000000 nibe-2.8.0/nibe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-05 08:41:53.000000 nibe-2.8.0/nibe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 08:41:53.000000 nibe-2.8.0/nibe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 08:41:53.000000 nibe-2.8.0/nibe.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-05 08:41:44.000000 nibe-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-05 08:41:53.989760 nibe-2.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 08:41:53.989760 nibe-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-02-05 08:41:44.000000 nibe-2.8.0/tests/test_coil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-02-05 08:41:44.000000 nibe-2.8.0/tests/test_heatpump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:22.368948 nibe-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-27 07:41:14.000000 nibe-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43802 2024-02-27 07:41:22.368948 nibe-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-02-27 07:41:14.000000 nibe-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:22.356948 nibe-2.9.0/nibe/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/coil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/coil_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:22.356948 nibe-2.9.0/nibe/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/connection/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/connection/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/connection/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25848 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/connection/nibegw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:22.360947 nibe-2.9.0/nibe/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/console_scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/console_scripts/convert_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:22.364947 nibe-2.9.0/nibe/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)   349721 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/f1145_f1245.json
+-rw-r--r--   0 runner    (1001) docker     (127)   235931 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/f1155_f1255.json
+-rw-r--r--   0 runner    (1001) docker     (127)   363565 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/f1345.json
+-rw-r--r--   0 runner    (1001) docker     (127)   371025 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/f1355.json
+-rw-r--r--   0 runner    (1001) docker     (127)   112411 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/f370_f470.json
+-rw-r--r--   0 runner    (1001) docker     (127)   133359 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/f730.json
+-rw-r--r--   0 runner    (1001) docker     (127)   149861 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/f750.json
+-rw-r--r--   0 runner    (1001) docker     (127)   257358 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/s1155_s1255.json
+-rw-r--r--   0 runner    (1001) docker     (127)   152644 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/s2125.json
+-rw-r--r--   0 runner    (1001) docker     (127)   167771 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/s320_s325.json
+-rw-r--r--   0 runner    (1001) docker     (127)   184019 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/s735.json
+-rw-r--r--   0 runner    (1001) docker     (127)    81925 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/smo20.json
+-rw-r--r--   0 runner    (1001) docker     (127)   302355 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/smo40.json
+-rw-r--r--   0 runner    (1001) docker     (127)   243617 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/smos40.json
+-rw-r--r--   0 runner    (1001) docker     (127)   210942 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/vvm225_vvm320_vvm325.json
+-rw-r--r--   0 runner    (1001) docker     (127)   206202 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/data/vvm310_vvm500.json
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/event_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/heatpump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:14.000000 nibe-2.9.0/nibe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:22.368948 nibe-2.9.0/nibe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43802 2024-02-27 07:41:22.000000 nibe-2.9.0/nibe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-27 07:41:22.000000 nibe-2.9.0/nibe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 07:41:22.000000 nibe-2.9.0/nibe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-27 07:41:22.000000 nibe-2.9.0/nibe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-27 07:41:22.000000 nibe-2.9.0/nibe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-27 07:41:22.000000 nibe-2.9.0/nibe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 07:41:22.000000 nibe-2.9.0/nibe.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-27 07:41:14.000000 nibe-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-27 07:41:22.368948 nibe-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 07:41:22.364947 nibe-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-02-27 07:41:14.000000 nibe-2.9.0/tests/test_coil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-02-27 07:41:14.000000 nibe-2.9.0/tests/test_heatpump.py
```

### Comparing `nibe-2.8.0/LICENSE` & `nibe-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/PKG-INFO` & `nibe-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibe
-Version: 2.8.0
+Version: 2.9.0
 Summary: Nibe heatpump communication library
 Home-page: https://github.com/yozik04/nibe
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/nibe/issues
 Keywords: nibe modbus library nibegw
```

### Comparing `nibe-2.8.0/README.md` & `nibe-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/coil.py` & `nibe-2.9.0/nibe/coil.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/coil_groups.py` & `nibe-2.9.0/nibe/coil_groups.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/connection/__init__.py` & `nibe-2.9.0/nibe/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/connection/encoders.py` & `nibe-2.9.0/nibe/connection/encoders.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/connection/mixins.py` & `nibe-2.9.0/nibe/connection/mixins.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/connection/modbus.py` & `nibe-2.9.0/nibe/connection/modbus.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/connection/nibegw.py` & `nibe-2.9.0/nibe/connection/nibegw.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/console_scripts/cli.py` & `nibe-2.9.0/nibe/console_scripts/cli.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/console_scripts/convert_csv.py` & `nibe-2.9.0/nibe/console_scripts/convert_csv.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/data/extensions.json` & `nibe-2.9.0/nibe/data/extensions.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9564855072463768%*

 * *Differences: {'0': "{'data': {'47340': {'mappings': {'18': 'BT74'}}}}",*

 * * 'insert': "[(22, OrderedDict([('description', 'Correction for BT71 missing in F1155/F1255'), "*

 * *           "('files', ['f1155_f1255.json']), ('data', OrderedDict([('40152', "*

 * *           "OrderedDict([('title', 'BT71 Ext. Return Temp'), ('info', 'External return "*

 * *           "temperature, BT71'), ('unit', '°C'), ('size', 's16'), ('factor', 10), ('name', "*

 * *           "'bt71-ext-return-temp-40152')]))]))]))]"}*

```diff
@@ -15,14 +15,15 @@
             },
             "47340": {
                 "factor": 1,
                 "mappings": {
                     "0": "OFF",
                     "1": "ON",
                     "10": "RMU-BT50",
+                    "18": "BT74",
                     "2": "BT50"
                 },
                 "max": 18.0
             },
             "47385": {
                 "mappings": {
                     "24": "24 hours"
@@ -492,9 +493,25 @@
                 "write": true
             }
         },
         "description": "Holiday settings",
         "files": [
             "f750.json"
         ]
+    },
+    {
+        "data": {
+            "40152": {
+                "factor": 10,
+                "info": "External return temperature, BT71",
+                "name": "bt71-ext-return-temp-40152",
+                "size": "s16",
+                "title": "BT71 Ext. Return Temp",
+                "unit": "\u00b0C"
+            }
+        },
+        "description": "Correction for BT71 missing in F1155/F1255",
+        "files": [
+            "f1155_f1255.json"
+        ]
     }
 ]
```

### Comparing `nibe-2.8.0/nibe/data/f1145_f1245.json` & `nibe-2.9.0/nibe/data/f1145_f1245.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999967298888162%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -8945,14 +8945,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/f1155_f1255.json` & `nibe-2.9.0/nibe/data/f1155_f1255.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998971340839304%*

 * *Differences: {"'40152'": "OrderedDict([('title', 'BT71 Ext. Return Temp'), ('info', 'External return "*

 * *            "temperature, BT71'), ('unit', '°C'), ('size', 's16'), ('factor', 10), ('name', "*

 * *            "'bt71-ext-return-temp-40152')])",*

 * * "'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -421,14 +421,22 @@
         "factor": 10,
         "info": "Hot water comfort supply temperature, BT70",
         "name": "bt70-hw-comfort-supply-temp-40147",
         "size": "s16",
         "title": "BT70 HW Comfort Supply Temp.",
         "unit": "\u00b0C"
     },
+    "40152": {
+        "factor": 10,
+        "info": "External return temperature, BT71",
+        "name": "bt71-ext-return-temp-40152",
+        "size": "s16",
+        "title": "BT71 Ext. Return Temp",
+        "unit": "\u00b0C"
+    },
     "40155": {
         "factor": 10,
         "info": "External collector temperature, BT57, for ACS",
         "name": "eq1-bt57-collector-temp-40155",
         "size": "s16",
         "title": "EQ1-BT57 Collector Temp.",
         "unit": "\u00b0C"
@@ -4731,14 +4739,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/f1345.json` & `nibe-2.9.0/nibe/data/f1345.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999968294229549%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -9337,14 +9337,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/f1355.json` & `nibe-2.9.0/nibe/data/f1355.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999969268592501%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -9496,14 +9496,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/f370_f470.json` & `nibe-2.9.0/nibe/data/f370_f470.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999897750511247%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -3080,14 +3080,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/f730.json` & `nibe-2.9.0/nibe/data/f730.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999913644214162%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -3549,14 +3549,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/f750.json` & `nibe-2.9.0/nibe/data/f750.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999922600619195%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -3940,14 +3940,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/s1155_s1255.json` & `nibe-2.9.0/nibe/data/s1155_s1255.json`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/data/s2125.json` & `nibe-2.9.0/nibe/data/s2125.json`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/data/s320_s325.json` & `nibe-2.9.0/nibe/data/s320_s325.json`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/data/s735.json` & `nibe-2.9.0/nibe/data/s735.json`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/data/smo20.json` & `nibe-2.9.0/nibe/data/smo20.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999864498644987%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -2376,14 +2376,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/smo40.json` & `nibe-2.9.0/nibe/data/smo40.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999962264150942%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -7168,14 +7168,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/smos40.json` & `nibe-2.9.0/nibe/data/smos40.json`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/data/vvm225_vvm320_vvm325.json` & `nibe-2.9.0/nibe/data/vvm225_vvm320_vvm325.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999943438914027%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -4485,14 +4485,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/data/vvm310_vvm500.json` & `nibe-2.9.0/nibe/data/vvm310_vvm500.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999942196531793%*

 * *Differences: {"'47340'": "{'mappings': {'18': 'BT74'}}"}*

```diff
@@ -4396,14 +4396,15 @@
         "default": 0.0,
         "factor": 1,
         "info": "Enables use of room sensor together with cooling 0=Off 1=On",
         "mappings": {
             "0": "OFF",
             "1": "ON",
             "10": "RMU-BT50",
+            "18": "BT74",
             "2": "BT50"
         },
         "max": 18.0,
         "min": 0.0,
         "name": "cooling-with-room-sensor-47340",
         "size": "u8",
         "title": "Cooling with room sensor",
```

### Comparing `nibe-2.8.0/nibe/event_server.py` & `nibe-2.9.0/nibe/event_server.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/exceptions.py` & `nibe-2.9.0/nibe/exceptions.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/heatpump.py` & `nibe-2.9.0/nibe/heatpump.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe/parsers.py` & `nibe-2.9.0/nibe/parsers.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/nibe.egg-info/PKG-INFO` & `nibe-2.9.0/nibe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibe
-Version: 2.8.0
+Version: 2.9.0
 Summary: Nibe heatpump communication library
 Home-page: https://github.com/yozik04/nibe
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/nibe/issues
 Keywords: nibe modbus library nibegw
```

### Comparing `nibe-2.8.0/nibe.egg-info/SOURCES.txt` & `nibe-2.9.0/nibe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/setup.cfg` & `nibe-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/tests/test_coil.py` & `nibe-2.9.0/tests/test_coil.py`

 * *Files identical despite different names*

### Comparing `nibe-2.8.0/tests/test_heatpump.py` & `nibe-2.9.0/tests/test_heatpump.py`

 * *Files identical despite different names*

