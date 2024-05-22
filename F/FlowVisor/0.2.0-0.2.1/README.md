# Comparing `tmp/FlowVisor-0.2.0.tar.gz` & `tmp/FlowVisor-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.2.0.tar", last modified: Mon May 20 18:19:30 2024, max compression
+gzip compressed data, was "FlowVisor-0.2.1.tar", last modified: Wed May 22 09:46:27 2024, max compression
```

## Comparing `FlowVisor-0.2.0.tar` & `FlowVisor-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.369689 FlowVisor-0.2.0/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.365689 FlowVisor-0.2.0/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.2.0/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-20 18:19:30.369689 FlowVisor-0.2.0/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3055 2024-05-13 12:49:23.000000 FlowVisor-0.2.0/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.365689 FlowVisor-0.2.0/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.2.0/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.365689 FlowVisor-0.2.0/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.2.0/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.2.0/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.2.0/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1172 2024-05-20 18:19:00.000000 FlowVisor-0.2.0/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    14811 2024-05-20 18:08:31.000000 FlowVisor-0.2.0/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2350 2024-05-20 17:44:05.000000 FlowVisor-0.2.0/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     7861 2024-05-13 12:26:30.000000 FlowVisor-0.2.0/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8494 2024-05-13 10:38:59.000000 FlowVisor-0.2.0/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.2.0/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.2.0/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.2.0/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2288 2024-05-20 18:08:09.000000 FlowVisor-0.2.0/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.2.0/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.2.0/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-20 18:19:30.369689 FlowVisor-0.2.0/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.2.0/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 09:46:27.295464 FlowVisor-0.2.1/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 09:46:27.295464 FlowVisor-0.2.1/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-22 09:46:27.000000 FlowVisor-0.2.1/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-22 09:46:27.000000 FlowVisor-0.2.1/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-22 09:46:27.000000 FlowVisor-0.2.1/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-22 09:46:27.000000 FlowVisor-0.2.1/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-05-22 09:46:27.000000 FlowVisor-0.2.1/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-22 09:46:27.000000 FlowVisor-0.2.1/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.2.1/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-22 09:46:27.295464 FlowVisor-0.2.1/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3055 2024-05-13 12:49:23.000000 FlowVisor-0.2.1/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 09:46:27.295464 FlowVisor-0.2.1/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.2.1/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 09:46:27.295464 FlowVisor-0.2.1/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.2.1/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.2.1/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.2.1/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1172 2024-05-20 18:19:00.000000 FlowVisor-0.2.1/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    14811 2024-05-20 18:08:31.000000 FlowVisor-0.2.1/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2350 2024-05-20 17:44:05.000000 FlowVisor-0.2.1/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8076 2024-05-22 09:41:15.000000 FlowVisor-0.2.1/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8494 2024-05-13 10:38:59.000000 FlowVisor-0.2.1/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.2.1/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.2.1/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.2.1/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2288 2024-05-20 18:08:09.000000 FlowVisor-0.2.1/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.2.1/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.2.1/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-22 09:46:27.295464 FlowVisor-0.2.1/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.2.1/setup.py
```

### Comparing `FlowVisor-0.2.0/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.2.1/FlowVisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.2.0
+Version: 0.2.1
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.2.0/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.2.1/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/LICENSE` & `FlowVisor-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/PKG-INFO` & `FlowVisor-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.2.0
+Version: 0.2.1
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.2.0/README.md` & `FlowVisor-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/cli/add_vis.py` & `FlowVisor-0.2.1/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/cli/remove_vis.py` & `FlowVisor-0.2.1/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/cli/vis_file.py` & `FlowVisor-0.2.1/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/flowvisor.py` & `FlowVisor-0.2.1/flowvisor/flowvisor.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/flowvisor_config.py` & `FlowVisor-0.2.1/flowvisor/flowvisor_config.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.2.1/flowvisor/flowvisor_verifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,28 +74,28 @@
 
     @staticmethod
     def export(file_name: str):
         """
         Export the verifier entries to a file
         """
         new_entries = FlowVisorVerifier.summaries_entries(FlowVisorVerifier.ENTRIES)
+
         device_name = utils.get_device_name()
         meta = {"device_name": device_name, "count": 0}
         old_data = None
 
         existing_content = FlowVisorVerifier.read_existing_file(file_name)
 
         if existing_content is not None:
             meta = existing_content["meta"]
             old_data = existing_content["data"]
-            new_entries = FlowVisorVerifier.avarage_entries(
-                old_data, new_entries, meta["count"]
-            )
 
+        new_entries = FlowVisorVerifier.add_trace(old_data, new_entries)
         new_entries = FlowVisorVerifier.set_min_max(old_data, new_entries)
+        new_entries = FlowVisorVerifier.avarage_entries(new_entries)
 
         # parse meta data
         meta["count"] += 1
         ex_device_name = meta["device_name"]
         if device_name not in ex_device_name:
             meta["device_name"] = f"{ex_device_name};;{device_name}"
         content = {
@@ -103,31 +103,21 @@
             "data": new_entries,
         }
 
         with open(file_name, "w", encoding="utf-8") as f:
             json.dump(content, f, indent=4)
 
     @staticmethod
-    def avarage_entries(old_data, new_data, count):
+    def avarage_entries(entries):
         """
         Avergae the entries
         """
-        for entry in new_data:
-            id_exists = False
-            for old_entry in old_data:
-                if old_entry["id"] == entry["id"]:
-                    old_entry["time"] = (old_entry["time"] * count + entry["time"]) / (
-                        count + 1
-                    )
-                    id_exists = True
-                    break
-            if not id_exists:
-                old_data.append(entry)
-
-        return old_data
+        for entry in entries:
+            entry["time"] = sum(entry["trace"]) / len(entry["trace"])
+        return entries
 
     @staticmethod
     def set_min_max(old_data, new_data):
         """
         Sets the min and max values for the entries
 
         Args:
@@ -148,14 +138,32 @@
                 if old_entry["id"] == entry["id"]:
                     entry["min"] = min(old_entry["min"], entry["time"])
                     entry["max"] = max(old_entry["max"], entry["time"])
                     break
         return new_data
 
     @staticmethod
+    def add_trace(old_data, new_data):
+        """
+        Add the time trace to the data
+        """
+        if old_data is None:
+            for entry in new_data:
+                entry["trace"] = [entry["time"]]
+            return new_data
+
+        for entry in new_data:
+            for old_entry in old_data:
+                if old_entry["id"] == entry["id"]:
+                    entry["trace"] = old_entry["trace"]
+                    entry["trace"].append(entry["time"])
+                    break
+        return new_data
+
+    @staticmethod
     def verify(nodes: List[FunctionNode], verify_file_name: str, threshold: float):
         verify_file_name = utils.apply_file_end(verify_file_name, "json")
 
         if not os.path.exists(verify_file_name):
             Logger.log(f"Verify file {verify_file_name} not found...")
             return
```

### Comparing `FlowVisor-0.2.0/flowvisor/function_node.py` & `FlowVisor-0.2.1/flowvisor/function_node.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/logger.py` & `FlowVisor-0.2.1/flowvisor/logger.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/sankey.py` & `FlowVisor-0.2.1/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/time_tracker.py` & `FlowVisor-0.2.1/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/time_value.py` & `FlowVisor-0.2.1/flowvisor/time_value.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/flowvisor/utils.py` & `FlowVisor-0.2.1/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.0/setup.py` & `FlowVisor-0.2.1/setup.py`

 * *Files identical despite different names*

