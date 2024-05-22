# Comparing `tmp/dashpool_components-0.0.8.tar.gz` & `tmp/dashpool_components-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashpool_components-0.0.8.tar", last modified: Sat Oct  7 19:07:32 2023, max compression
+gzip compressed data, was "dashpool_components-0.0.9.tar", last modified: Sat Oct  7 20:38:35 2023, max compression
```

## Comparing `dashpool_components-0.0.8.tar` & `dashpool_components-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 19:07:32.031778 dashpool_components-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-07 19:06:25.000000 dashpool_components-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-07 19:06:25.000000 dashpool_components-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-07 19:07:32.031778 dashpool_components-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-07 19:06:25.000000 dashpool_components-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 19:07:32.031778 dashpool_components-0.0.8/dashpool_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components/DashpoolProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components/Explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components/History.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components/Loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-10-07 19:07:20.000000 dashpool_components-0.0.8/dashpool_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)   501346 2023-10-07 19:07:28.000000 dashpool_components-0.0.8/dashpool_components/dashpool_components.js
--rw-r--r--   0 runner    (1001) docker     (127)    17764 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-10-07 19:07:29.000000 dashpool_components-0.0.8/dashpool_components/package-info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 19:07:32.031778 dashpool_components-0.0.8/dashpool_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-07 19:07:31.000000 dashpool_components-0.0.8/dashpool_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-07 19:07:32.031778 dashpool_components-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-07 19:06:25.000000 dashpool_components-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 20:38:35.668324 dashpool_components-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-07 20:37:11.000000 dashpool_components-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-07 20:37:11.000000 dashpool_components-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-07 20:38:35.664324 dashpool_components-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-07 20:37:11.000000 dashpool_components-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 20:38:35.664324 dashpool_components-0.0.9/dashpool_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-10-07 20:38:34.000000 dashpool_components-0.0.9/dashpool_components/DashpoolProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2023-10-07 20:38:34.000000 dashpool_components-0.0.9/dashpool_components/Explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-10-07 20:38:34.000000 dashpool_components-0.0.9/dashpool_components/History.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-10-07 20:38:34.000000 dashpool_components-0.0.9/dashpool_components/Loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-10-07 20:38:22.000000 dashpool_components-0.0.9/dashpool_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-07 20:38:34.000000 dashpool_components-0.0.9/dashpool_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (127)   501355 2023-10-07 20:38:30.000000 dashpool_components-0.0.9/dashpool_components/dashpool_components.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18289 2023-10-07 20:38:34.000000 dashpool_components-0.0.9/dashpool_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-10-07 20:38:31.000000 dashpool_components-0.0.9/dashpool_components/package-info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 20:38:35.664324 dashpool_components-0.0.9/dashpool_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-07 20:38:35.000000 dashpool_components-0.0.9/dashpool_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2023-10-07 20:38:35.000000 dashpool_components-0.0.9/dashpool_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 20:38:35.000000 dashpool_components-0.0.9/dashpool_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-07 20:38:35.000000 dashpool_components-0.0.9/dashpool_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-07 20:38:35.668324 dashpool_components-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-07 20:37:11.000000 dashpool_components-0.0.9/setup.py
```

### Comparing `dashpool_components-0.0.8/README.md` & `dashpool_components-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dashpool_components-0.0.8/dashpool_components/DashpoolProvider.py` & `dashpool_components-0.0.9/dashpool_components/DashpoolProvider.py`

 * *Files identical despite different names*

### Comparing `dashpool_components-0.0.8/dashpool_components/Explorer.py` & `dashpool_components-0.0.9/dashpool_components/Explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 
     - icon (string; optional)
 
     - id (string; required)
 
     - label (string; required)
 
+    - layout (string; optional)
+
     - parent (string; optional)
 
     - shared (list of strings; optional)
 
     - type (string; required)
 
 - nodes (list of dicts; required):
@@ -114,14 +116,16 @@
 
     - icon (string; optional)
 
     - id (string; required)
 
     - label (string; required)
 
+    - layout (string; optional)
+
     - parent (string; optional)
 
     - shared (list of strings; optional)
 
     - type (string; required)"""
     _children_props = []
     _base_nodes = ['children']
```

### Comparing `dashpool_components-0.0.8/dashpool_components/History.py` & `dashpool_components-0.0.9/dashpool_components/History.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 
     - icon (string; optional)
 
     - id (string; required)
 
     - label (string; required)
 
+    - layout (string; optional)
+
     - parent (string; optional)
 
     - shared (list of strings; optional)
 
     - type (string; required)"""
     _children_props = []
     _base_nodes = ['children']
```

### Comparing `dashpool_components-0.0.8/dashpool_components/Loader.py` & `dashpool_components-0.0.9/dashpool_components/Loader.py`

 * *Files identical despite different names*

### Comparing `dashpool_components-0.0.8/dashpool_components/__init__.py` & `dashpool_components-0.0.9/dashpool_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dashpool_components-0.0.8/dashpool_components/dashpool_components.js` & `dashpool_components-0.0.9/dashpool_components/dashpool_components.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7618,15 +7618,16 @@
                                             g({
                                                 dragElement: {
                                                     id: p,
                                                     type: "a",
                                                     label: c,
                                                     parent: "history",
                                                     app: c,
-                                                    frame: d
+                                                    frame: d,
+                                                    layout: p
                                                 }
                                             })
                                         })).catch((function(e) {
                                             console.error("There was a problem with the fetch operation:", e), g({
                                                 dragElement: {}
                                             })
                                         }))
```

### Comparing `dashpool_components-0.0.8/dashpool_components/metadata.json` & `dashpool_components-0.0.9/dashpool_components/metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999952377507716%*

 * *Differences: {"'src/ts/components/Explorer.tsx'": "{'props': {'nodes': {'type': {'value': {'value': {'layout': "*

 * *                                     "OrderedDict([('description', ''), ('required', False), "*

 * *                                     "('name', 'string'), ('raw', 'string')])}}}}, "*

 * *                                     "'nodeChangeEvent': {'type': {'value': {'layout': "*

 * *                                     "OrderedDict([('description', ''), ('required', False), "*

 * *                                     "('name', ' […]*

```diff
@@ -161,14 +161,20 @@
                         },
                         "label": {
                             "description": "",
                             "name": "string",
                             "raw": "string",
                             "required": true
                         },
+                        "layout": {
+                            "description": "",
+                            "name": "string",
+                            "raw": "string",
+                            "required": false
+                        },
                         "parent": {
                             "description": "",
                             "name": "string",
                             "raw": "string",
                             "required": false
                         },
                         "shared": {
@@ -232,14 +238,20 @@
                             },
                             "label": {
                                 "description": "",
                                 "name": "string",
                                 "raw": "string",
                                 "required": true
                             },
+                            "layout": {
+                                "description": "",
+                                "name": "string",
+                                "raw": "string",
+                                "required": false
+                            },
                             "parent": {
                                 "description": "",
                                 "name": "string",
                                 "raw": "string",
                                 "required": false
                             },
                             "shared": {
@@ -406,14 +418,20 @@
                             },
                             "label": {
                                 "description": "",
                                 "name": "string",
                                 "raw": "string",
                                 "required": true
                             },
+                            "layout": {
+                                "description": "",
+                                "name": "string",
+                                "raw": "string",
+                                "required": false
+                            },
                             "parent": {
                                 "description": "",
                                 "name": "string",
                                 "raw": "string",
                                 "required": false
                             },
                             "shared": {
```

### Comparing `dashpool_components-0.0.8/dashpool_components/package-info.json` & `dashpool_components-0.0.9/dashpool_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -40,9 +40,9 @@
         "build": "npm run build:init && npm run build:js && npm run build:backends",
         "build:backends": "dash-generate-components ./src/ts/components dashpool_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:init": "node -e \"const fs = require('fs-extra'); const sourceDir = 'dashpool_components_base'; const destDir = 'dashpool_components'; fs.ensureDirSync(destDir); fs.copySync(sourceDir, destDir, { overwrite: true }); console.log('Build:init script completed.');\"",
         "build:js": "webpack",
         "build:js::dev": "webpack --mode development",
         "watch": "npm run build:js::dev -- --watch"
     },
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

### Comparing `dashpool_components-0.0.8/dashpool_components.egg-info/SOURCES.txt` & `dashpool_components-0.0.9/dashpool_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashpool_components-0.0.8/setup.py` & `dashpool_components-0.0.9/setup.py`

 * *Files identical despite different names*

