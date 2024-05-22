# Comparing `tmp/funcnodes-0.2.8.tar.gz` & `tmp/funcnodes-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes-0.2.8.tar", max compression
+gzip compressed data, was "funcnodes-0.2.9.tar", max compression
```

## Comparing `funcnodes-0.2.8.tar` & `funcnodes-0.2.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1787 2024-05-14 12:52:21.747900 funcnodes-0.2.8/funcnodes/__init__.py
--rw-r--r--   0        0        0     6736 2024-05-14 12:22:29.469309 funcnodes-0.2.8/funcnodes/__main__.py
--rw-r--r--   0        0        0     2476 2024-05-14 12:14:27.351209 funcnodes-0.2.8/funcnodes/_logging.py
--rw-r--r--   0        0        0      278 2024-05-14 07:14:15.014932 funcnodes-0.2.8/funcnodes/basic_nodes/__init__.py
--rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.8/funcnodes/basic_nodes/logic.py
--rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.8/funcnodes/basic_nodes/math.py
--rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.8/funcnodes/config.py
--rw-r--r--   0        0        0     1911 2024-05-08 18:44:35.771663 funcnodes-0.2.8/funcnodes/data.py
--rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.8/funcnodes/eventmanager.py
--rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.8/funcnodes/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.8/funcnodes/frontends/__init__.py
--rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/asset-manifest.json
--rw-r--r--   0        0        0    29231 2024-05-14 07:55:51.314737 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/css/style.css
--rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/favicon.ico
--rw-r--r--   0        0        0      763 2024-05-14 08:01:24.659745 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/index.html
--rw-r--r--   0        0        0  4149018 2024-05-14 07:55:51.316736 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js
--rw-r--r--   0        0        0     3258 2024-05-14 07:55:51.313726 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt
--rw-r--r--   0        0        0   256239 2024-05-14 07:55:51.314737 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js
--rw-r--r--   0        0        0    11501 2024-05-14 07:55:51.314737 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
--rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo192.png
--rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo512.png
--rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/manifest.json
--rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/robots.txt
--rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/run.py
--rw-r--r--   0        0        0      323 2024-05-10 14:51:11.297311 funcnodes-0.2.8/funcnodes/graph.py
--rw-r--r--   0        0        0    29347 2024-05-14 10:50:19.461839 funcnodes-0.2.8/funcnodes/io.py
--rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.8/funcnodes/lib/__init__.py
--rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.8/funcnodes/lib/lib.py
--rw-r--r--   0        0        0     7259 2024-05-11 04:44:57.813753 funcnodes-0.2.8/funcnodes/lib/libfinder.py
--rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.8/funcnodes/lib/libparser.py
--rw-r--r--   0        0        0    35376 2024-05-14 12:54:42.228979 funcnodes-0.2.8/funcnodes/node.py
--rw-r--r--   0        0        0    20423 2024-05-14 07:16:32.158888 funcnodes-0.2.8/funcnodes/nodemaker.py
--rw-r--r--   0        0        0    11850 2024-05-11 05:25:23.856740 funcnodes-0.2.8/funcnodes/nodespace.py
--rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.8/funcnodes/triggerstack.py
--rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.8/funcnodes/utils/__init__.py
--rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.8/funcnodes/utils/data.py
--rw-r--r--   0        0        0     2744 2024-05-14 07:12:12.066097 funcnodes-0.2.8/funcnodes/utils/nodeutils.py
--rw-r--r--   0        0        0     5994 2024-05-14 09:16:47.009589 funcnodes-0.2.8/funcnodes/utils/serialization.py
--rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.8/funcnodes/worker/__init__.py
--rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.8/funcnodes/worker/external_worker.py
--rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.8/funcnodes/worker/loop.py
--rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.8/funcnodes/worker/remote_worker.py
--rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.8/funcnodes/worker/websocket.py
--rw-r--r--   0        0        0    38268 2024-05-14 12:15:05.691889 funcnodes-0.2.8/funcnodes/worker/worker.py
--rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.8/funcnodes/worker/worker_manager.py
--rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.8/LICENSE
--rw-r--r--   0        0        0      694 2024-05-14 12:52:09.360725 funcnodes-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.8/README.md
--rw-r--r--   0        0        0    13535 1970-01-01 00:00:00.000000 funcnodes-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1787 2024-05-14 13:16:53.678069 funcnodes-0.2.9/funcnodes/__init__.py
+-rw-r--r--   0        0        0     6769 2024-05-14 13:00:18.581806 funcnodes-0.2.9/funcnodes/__main__.py
+-rw-r--r--   0        0        0     2476 2024-05-14 12:14:27.351209 funcnodes-0.2.9/funcnodes/_logging.py
+-rw-r--r--   0        0        0      278 2024-05-14 07:14:15.014932 funcnodes-0.2.9/funcnodes/basic_nodes/__init__.py
+-rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.9/funcnodes/basic_nodes/logic.py
+-rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.9/funcnodes/basic_nodes/math.py
+-rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.9/funcnodes/config.py
+-rw-r--r--   0        0        0     1911 2024-05-08 18:44:35.771663 funcnodes-0.2.9/funcnodes/data.py
+-rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.9/funcnodes/eventmanager.py
+-rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.9/funcnodes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.9/funcnodes/frontends/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/asset-manifest.json
+-rw-r--r--   0        0        0    29231 2024-05-14 07:55:51.314737 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/css/style.css
+-rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/favicon.ico
+-rw-r--r--   0        0        0      763 2024-05-14 08:01:24.659745 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/index.html
+-rw-r--r--   0        0        0  4149018 2024-05-14 07:55:51.316736 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/743.js
+-rw-r--r--   0        0        0     3258 2024-05-14 07:55:51.313726 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt
+-rw-r--r--   0        0        0   256239 2024-05-14 07:55:51.314737 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/main.js
+-rw-r--r--   0        0        0    11501 2024-05-14 07:55:51.314737 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
+-rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/logo192.png
+-rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/logo512.png
+-rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/manifest.json
+-rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/robots.txt
+-rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/run.py
+-rw-r--r--   0        0        0      323 2024-05-10 14:51:11.297311 funcnodes-0.2.9/funcnodes/graph.py
+-rw-r--r--   0        0        0    29440 2024-05-14 13:13:30.784719 funcnodes-0.2.9/funcnodes/io.py
+-rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.9/funcnodes/lib/__init__.py
+-rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.9/funcnodes/lib/lib.py
+-rw-r--r--   0        0        0     7259 2024-05-11 04:44:57.813753 funcnodes-0.2.9/funcnodes/lib/libfinder.py
+-rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.9/funcnodes/lib/libparser.py
+-rw-r--r--   0        0        0    35518 2024-05-14 13:16:08.185855 funcnodes-0.2.9/funcnodes/node.py
+-rw-r--r--   0        0        0    20423 2024-05-14 07:16:32.158888 funcnodes-0.2.9/funcnodes/nodemaker.py
+-rw-r--r--   0        0        0    11850 2024-05-11 05:25:23.856740 funcnodes-0.2.9/funcnodes/nodespace.py
+-rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.9/funcnodes/triggerstack.py
+-rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.9/funcnodes/utils/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.9/funcnodes/utils/data.py
+-rw-r--r--   0        0        0     2744 2024-05-14 07:12:12.066097 funcnodes-0.2.9/funcnodes/utils/nodeutils.py
+-rw-r--r--   0        0        0     5994 2024-05-14 09:16:47.009589 funcnodes-0.2.9/funcnodes/utils/serialization.py
+-rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.9/funcnodes/worker/__init__.py
+-rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.9/funcnodes/worker/external_worker.py
+-rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.9/funcnodes/worker/loop.py
+-rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.9/funcnodes/worker/remote_worker.py
+-rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.9/funcnodes/worker/websocket.py
+-rw-r--r--   0        0        0    38268 2024-05-14 12:15:05.691889 funcnodes-0.2.9/funcnodes/worker/worker.py
+-rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.9/funcnodes/worker/worker_manager.py
+-rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.9/LICENSE
+-rw-r--r--   0        0        0      694 2024-05-14 13:17:02.371766 funcnodes-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.9/README.md
+-rw-r--r--   0        0        0    13535 1970-01-01 00:00:00.000000 funcnodes-0.2.9/PKG-INFO
```

### Comparing `funcnodes-0.2.8/funcnodes/__init__.py` & `funcnodes-0.2.9/funcnodes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,10 +65,10 @@
     "config",
     "RenderOptions",
     "NoValue",
     "DataEnum",
     "add_type",
 ]
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 DEBUG = True
```

### Comparing `funcnodes-0.2.8/funcnodes/__main__.py` & `funcnodes-0.2.9/funcnodes/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import Type
 from funcnodes.frontends.funcnodes_react import run_server
 import funcnodes as fn
 import argparse
 from pprint import pprint
 import sys
 import os
-import setproctitle
+
+try:
+    from setproctitle import setproctitle
+except ModuleNotFoundError:
+    setproctitle = print
 
 
 def task_run_server(args: argparse.Namespace):
     """
     Runs the server.
 
     Args:
@@ -18,15 +22,15 @@
     Returns:
       None
 
     Examples:
       >>> task_run_server(args)
       None
     """
-    setproctitle.setproctitle("funcnodes_server")
+    setproctitle("funcnodes_server")
     run_server(port=args.port, open_browser=args.no_browser)
 
 
 def list_workers(args: argparse.Namespace):
     """
     Lists all workers.
 
@@ -62,15 +66,15 @@
       >>> start_new_worker(args)
       None
     """
     worker_class: Type[fn.worker.Worker] = getattr(fn.worker, args.workertype)
     fn.FUNCNODES_LOGGER.info(f"Starting new worker of type {args.workertype}")
 
     worker = worker_class(uuid=args.uuid, name=args.name)
-    setproctitle.setproctitle("worker " + worker.uuid())
+    setproctitle("worker " + worker.uuid())
     worker.run_forever()
 
 
 def start_existing_worker(args: argparse.Namespace):
     """
     Starts an existing worker.
 
@@ -119,15 +123,15 @@
         if not os.path.exists(cfg["python_path"]):
             raise Exception(f"Python executable not found: {cfg['python_path']}")
         os.execv(cfg["python_path"], ["-m", "funcnodes"] + sys.argv[1:])
 
     fn.FUNCNODES_LOGGER.info(f"Starting existing worker of type {args.workertype}")
     worker = worker_class(uuid=cfg["uuid"])
 
-    setproctitle.setproctitle("worker " + worker.uuid())
+    setproctitle("worker " + worker.uuid())
     worker.run_forever()
 
 
 def task_worker(args: argparse.Namespace):
     """
     Performs a task on worker(s).
 
@@ -166,15 +170,15 @@
     Returns:
       None
 
     Examples:
       >>> start_worker_manager(args)
       None
     """
-    setproctitle.setproctitle("worker_manager")
+    setproctitle("worker_manager")
     fn.worker.worker_manager.start_worker_manager()
 
 
 def main():
     """
     The main function.
```

### Comparing `funcnodes-0.2.8/funcnodes/_logging.py` & `funcnodes-0.2.9/funcnodes/_logging.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/basic_nodes/logic.py` & `funcnodes-0.2.9/funcnodes/basic_nodes/logic.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/basic_nodes/math.py` & `funcnodes-0.2.9/funcnodes/basic_nodes/math.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/config.py` & `funcnodes-0.2.9/funcnodes/config.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/data.py` & `funcnodes-0.2.9/funcnodes/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/eventmanager.py` & `funcnodes-0.2.9/funcnodes/eventmanager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/asset-manifest.json` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/css/style.css` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/css/style.css`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/favicon.ico` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/favicon.ico`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/index.html` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/index.html`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/743.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/main.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo192.png` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/logo192.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo512.png` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/logo512.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/run.py` & `funcnodes-0.2.9/funcnodes/frontends/funcnodes_react/run.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/io.py` & `funcnodes-0.2.9/funcnodes/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         if "description" in data:
             self._description = data["description"]
         if "id" in data:
             self._uuid = data["id"]
         if "value" in data:
             self._value = data["value"]
 
-    def serialize(self) -> NodeIOSerialization:
+    def serialize(self, drop=True) -> NodeIOSerialization:
         """Serializes the NodeIO instance to a dictionary.
 
         Returns:
             A dictionary containing the serialized name and description.
         """
         ser = NodeIOSerialization(
             name=self._name,
@@ -371,22 +371,23 @@
             ser["description"] = self._description
         if (
             self.allow_multiple is not None
             and self.allow_multiple is not self.default_allow_multiple
         ):
             ser["allow_multiple"] = self.allow_multiple
 
-        if ser["name"] == ser["id"]:
-            del ser["name"]
+        if drop:
+            if ser["name"] == ser["id"]:
+                del ser["name"]
 
-        if len(ser["render_options"]) == 0:
-            del ser["render_options"]
+            if len(ser["render_options"]) == 0:
+                del ser["render_options"]
 
-        if len(ser["value_options"]) == 0:
-            del ser["value_options"]
+            if len(ser["value_options"]) == 0:
+                del ser["value_options"]
 
         return ser
 
     @property
     def name(self) -> str:
         """Gets the name of the NodeIO."""
         return self._name
@@ -728,23 +729,23 @@
             uuid=serialized_input["name"],
             description=serialized_input.get("description"),
             type=serialized_input["type"],
             allow_multiple=serialized_input.get("allow_multiple"),
             default=serialized_input.get("default", NoValue),
         )
 
-    def serialize(self) -> NodeInputSerialization:
+    def serialize(self, drop=True) -> NodeInputSerialization:
         """
         Serializes the NodeInput instance to a dictionary for storage or transmission.
 
         Returns:
             A dictionary containing the serialized name and description of the node input.
         """
         ser = NodeInputSerialization(
-            **super().serialize(),
+            **super().serialize(drop=drop),
         )
         if self.required is not NodeInput.default_required:
             ser["required"] = self.required
         if self.does_trigger is not NodeInput.default_does_trigger:
             ser["does_trigger"] = self.does_trigger
         if self._default is not NoValue:
             ser["default"] = self._default
@@ -753,15 +754,15 @@
             and not self.is_connected()  # value is stored only if not connected
         ):
             ser["value"] = self.value
         return ser
 
     def to_dict(self) -> NodeInputOptions:
         ser: IOOptions = NodeInputOptions(
-            **self.serialize(),
+            **self.serialize(drop=False),
         )
         return ser
 
     def deserialize(self, data: NodeInputSerialization) -> None:
         super().deserialize(data)
         if "required" in data:
             self.required = data["required"]
@@ -891,15 +892,15 @@
         Returns:
             A dictionary containing the serialized name and description of the node output.
         """
         return NodeOutputSerialization(**super().serialize())
 
     def to_dict(self) -> NodeOutputOptions:
         ser: IOOptions = NodeOutputOptions(
-            **self.serialize(),
+            **self.serialize(drop=False),
         )
         return ser
 
     def deserialize(self, data: NodeIOSerialization) -> None:
         return super().deserialize(data)
 
     @classmethod
```

### Comparing `funcnodes-0.2.8/funcnodes/lib/lib.py` & `funcnodes-0.2.9/funcnodes/lib/lib.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/lib/libfinder.py` & `funcnodes-0.2.9/funcnodes/lib/libfinder.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/lib/libparser.py` & `funcnodes-0.2.9/funcnodes/lib/libparser.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/node.py` & `funcnodes-0.2.9/funcnodes/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             ip.uuid, {}
         )
 
         node_io_options: NodeInputOptions = node.io_options.get(ip.uuid, {})
 
         if node_io_render:
             deep_fill_dict(
-                ser["render_options"], node_io_render, overwrite_existing=True
+                ser.get("render_options", {}), node_io_render, overwrite_existing=True
             )
 
         if node_io_options:
             deep_fill_dict(ser, node_io_options, overwrite_existing=True)
 
         node.add_input(
             NodeInput(
@@ -430,15 +430,15 @@
                 if iod.uuid in data["io"]:
                     iod.deserialize(data["io"][iod.uuid])  # type: ignore
 
         if self.trigger_on_create:
             if self.ready_to_trigger():
                 self.request_trigger()
 
-    def serialize(self) -> NodeJSON:
+    def serialize(self, drop=True) -> NodeJSON:
         """
         returns a json serializable dict of the node
         """
 
         ser = NodeJSON(
             name=self.name,
             id=self.uuid,
@@ -446,45 +446,46 @@
             node_name=getattr(self, "node_name", self.__class__.__name__),
             io={},
         )
 
         for iod in self._inputs + self._outputs:
             if iod.uuid == "_triggerinput":
                 continue
-            ioser = dict(iod.serialize())
-            del ioser["id"]
-
-            cls_ser = None
-            if iod.uuid in self._class_io_serialized:
-                cls_ser = self._class_io_serialized[iod.uuid]
-
-            if cls_ser:
-                if "description" in ioser:
-                    if ioser["description"] == cls_ser.get("description", ""):
-                        del ioser["description"]
-
-                if "default" in ioser:
-                    if ioser["default"] == cls_ser.get("default", NoValue):
-                        del ioser["default"]
-
-                if "type" in ioser:
-                    if ioser["type"] == cls_ser.get("type", "Any"):
-                        del ioser["type"]
-
-                if "value_options" in ioser:
-                    if ioser["value_options"] == cls_ser.get("value_options", {}):
-                        del ioser["value_options"]
-
-                if "render_options" in ioser:
-                    if ioser["render_options"] == cls_ser.get("render_options", {}):
-                        del ioser["render_options"]
-
-                if "default" in ioser:
-                    if ioser["default"] == cls_ser.get("default", NoValue):
-                        del ioser["default"]
+            ioser = dict(iod.serialize(drop=drop))
+            if drop:
+                del ioser["id"]
+
+                cls_ser = None
+                if iod.uuid in self._class_io_serialized:
+                    cls_ser = self._class_io_serialized[iod.uuid]
+
+                if cls_ser:
+                    if "description" in ioser:
+                        if ioser["description"] == cls_ser.get("description", ""):
+                            del ioser["description"]
+
+                    if "default" in ioser:
+                        if ioser["default"] == cls_ser.get("default", NoValue):
+                            del ioser["default"]
+
+                    if "type" in ioser:
+                        if ioser["type"] == cls_ser.get("type", "Any"):
+                            del ioser["type"]
+
+                    if "value_options" in ioser:
+                        if ioser["value_options"] == cls_ser.get("value_options", {}):
+                            del ioser["value_options"]
+
+                    if "render_options" in ioser:
+                        if ioser["render_options"] == cls_ser.get("render_options", {}):
+                            del ioser["render_options"]
+
+                    if "default" in ioser:
+                        if ioser["default"] == cls_ser.get("default", NoValue):
+                            del ioser["default"]
 
             ser["io"][iod.uuid] = ioser
 
         if self.reset_inputs_on_trigger != self.default_reset_inputs_on_trigger:
             ser["reset_inputs_on_trigger"] = self.reset_inputs_on_trigger
 
         if self.description != self.__class__.description:
```

### Comparing `funcnodes-0.2.8/funcnodes/nodemaker.py` & `funcnodes-0.2.9/funcnodes/nodemaker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/nodespace.py` & `funcnodes-0.2.9/funcnodes/nodespace.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/triggerstack.py` & `funcnodes-0.2.9/funcnodes/triggerstack.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/utils/data.py` & `funcnodes-0.2.9/funcnodes/utils/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/utils/nodeutils.py` & `funcnodes-0.2.9/funcnodes/utils/nodeutils.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/utils/serialization.py` & `funcnodes-0.2.9/funcnodes/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/worker/external_worker.py` & `funcnodes-0.2.9/funcnodes/worker/external_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/worker/loop.py` & `funcnodes-0.2.9/funcnodes/worker/loop.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/worker/remote_worker.py` & `funcnodes-0.2.9/funcnodes/worker/remote_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/worker/websocket.py` & `funcnodes-0.2.9/funcnodes/worker/websocket.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/worker/worker.py` & `funcnodes-0.2.9/funcnodes/worker/worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/funcnodes/worker/worker_manager.py` & `funcnodes-0.2.9/funcnodes/worker/worker_manager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/LICENSE` & `funcnodes-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/pyproject.toml` & `funcnodes-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcnodes"
-version = "0.2.8"
+version = "0.2.9"
 description = "funcnodes"
 authors = ["Julian Kimmig <julian.kimmig@linkdlab.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 exposedfunctionality = ">=0.3.7"
```

### Comparing `funcnodes-0.2.8/README.md` & `funcnodes-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.8/PKG-INFO` & `funcnodes-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes
-Version: 0.2.8
+Version: 0.2.9
 Summary: funcnodes
 Author: Julian Kimmig
 Author-email: julian.kimmig@linkdlab.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

